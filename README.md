# kevin's 网页指南

静态版网页书签页。清单在 `records.csv`，页面运行时读取它渲染。

## 文件

- `index.html` —— 页面本体（单文件，样式和脚本都内联）
- `records.csv` —— 网址清单，列：`名称,网址,分类,描述,收录日期`

## 改内容

改 `records.csv` 即可（Excel、记事本都行，存为 UTF-8）。也可以让小布从资料库同步一份过来。

## 本地预览

浏览器直接双击 `index.html` 会读不到 CSV（被同源策略拦），起个本地服务就行：

```
python -m http.server 8000
```

然后开 http://localhost:8000 。
