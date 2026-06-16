# 更新網站的流程
修改內容 → 本機預覽與檢查 → git add → git commit → git push → GitHub Actions 自動部署

### 本機測試
```bash
mkdocs serve
mkdocs build
```

### 上傳至 GitHub
```bash
git add .
git commit -m "Update documentation"
git push
```
