# HeZhen's Blog

基于Hugo的AIOVTUE主题的个人博客

使用方法参考https://github.com/AIOVTUE/hugo-theme-aiovtue

## 本地开发与测试

```bash
cd hugo-theme-aiovtue

# 安装依赖（管理员运行）
pnpm install

# 启动网页
pnpm dev

# 浏览器打开
# http://localhost:1313
```

常用操作：

- 改文章 / 页面 → 保存后浏览器刷新
- 改 `hugo.toml` / `data/links.yaml` → 自动生效
- 按 `Ctrl+C` 停止服务器

### 本地构建（模拟上线产物）

```bash
pnpm build
```

构建结果在 `public/` 目录。`--cleanDestinationDir` 会先清空旧文件，避免已删文章残留。

本地预览构建结果（可选）：

```bash
npx --yes serve public
# 或任意静态文件服务器指向 public/
```

---

## 常用命令速查

```bash
pnpm dev     # 本地开发预览
pnpm build   # 构建到 public/（部署用）
```
