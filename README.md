# leap-zh.nvim

基于 [leap.nvim](https://github.com/ggandor/leap.nvim) 的中文词跳转, 双拼方案选择[小鹤双拼](https://flypy.com/)

## 安装

```lua
-- dependency 可以不要
  { 'noearc/leap-zh.nvim', dependencies = { 'noearc/jieba-lua' } }
```

## 键位

- 自行选择以下 function 要如何映射，示例：

```lua
map.set('n', 'fs', ":lua require'leap-zh'.leap_zh()<CR>") -- 向下搜索
map.set('n', 'fb', ":lua require'leap-zh'.leap_zh_bak()<CR>") -- 向上搜索
map.set('n', 'fw', ":lua require'leap-zh'.leap_jieba()<CR>") -- 搜索当前行的中文词
```

## TODO

- [ ] 处理中英混合文件
- [ ] 增加更多双排方案
