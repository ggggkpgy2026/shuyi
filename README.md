# 蜀一采购清单

一个纯前端的采购清单页面，可直接部署到 GitHub Pages。

## 功能

- 添加、编辑、删除采购商品
- 上传本地图片并预览
- 自动统计总金额、商品种类、总数量
- 导入/导出 JSON
- 导出 CSV
- Letter 横向彩色打印版

## 数据说明

数据默认保存在仓库根目录的 `data.json` 中。

页面打开时会自动读取 GitHub 上的 `data.json`。添加、编辑、删除后，先在页面内更新本地状态，再点击“保存到 Git”把当前清单提交回仓库。

保存到 Git 需要填写 GitHub fine-grained personal access token。建议只给这个仓库的 `Contents: Read and write` 权限。token 只保存在当前浏览器的 `localStorage` 中，不会写入仓库。

仍建议定期使用“导出 JSON”备份，需要迁移或恢复时可用“导入 JSON”。

## 部署

仓库根目录包含 `index.html`，可以直接用 GitHub Pages 从 `main` 分支根目录发布。
