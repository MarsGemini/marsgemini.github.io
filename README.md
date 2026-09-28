# Yiping Ma Academic Homepage

这是一套可直接发布到 GitHub Pages 的纯静态个人学术主页，不依赖 Node.js、Jekyll 或数据库。

## 文件结构

- `index.html`：个人简介、研究成果、科研项目、社会参与、荣誉和联系方式。
- `styles.css`：桌面端固定个人侧栏、右侧滚动内容及移动端适配。
- `assets/`：头像、论文缩略图和网页图标。
- `.nojekyll`：让 GitHub Pages 直接发布静态文件。

## 发布到 GitHub Pages

在 GitHub 新建公开仓库：

```text
marsgemini.github.io
```

然后在本文件夹运行：

```bash
git init
git add .
git commit -m "Create academic homepage"
git branch -M main
git remote add origin https://github.com/MarsGemini/marsgemini.github.io.git
git push -u origin main
```

进入仓库的 `Settings` → `Pages`，将发布方式设置为：

- Source：`Deploy from a branch`
- Branch：`main`
- Folder：`/(root)`

发布地址：`https://marsgemini.github.io/`

## 后续更新

主要内容都集中在 `index.html`。修改论文状态、增加成果或调整获奖信息后执行：

```bash
git add .
git commit -m "Update homepage"
git push
```
