### 常用命令

```shell
pnpm run server  # 启动服务器
pnpm run build   # 生成静态文件
pnpm run clean   # 清除缓存文件(db.json)和静态文件(public)
pnpx hexo new <title>  # 新建文章
```

### 语法高亮主题

`monokai`
`agate`
`tomorrow-night-blue`
`tomorrow-night-eighties`

### 主题bug修复

编辑 `themes/cactus/source/js/main.js`

```diff
// hide only the navigation links on desktop
-if (!nav.is(":visible") && topDistance < 50) {
+if (!nav.is(":visible") && topDistance < 150) {
  nav.show();
} else if (nav.is(":visible") && topDistance > 100) {
  nav.hide();
}
```