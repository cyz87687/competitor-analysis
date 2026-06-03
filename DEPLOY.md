# 部署到 GitHub Pages 指南

## 步骤 1：配置 Git 用户信息
```bash
git config --global user.name "你的GitHub用户名"
git config --global user.email "你的GitHub邮箱"
```

## 步骤 2：初始化 Git 仓库并提交
```bash
cd c:\cyz\工作文档\陈远卓\Python\article\LSTM_Stock-main\LSTM_Stock
git init
git add index.html vercel.json
git commit -m "feat: 竞品分析周报系统"
```

## 步骤 3：创建 GitHub 仓库并推送
1. 在 GitHub 网站上创建新仓库（如 `competitor-analysis`）
2. 执行：
```bash
git remote add origin https://github.com/你的用户名/competitor-analysis.git
git branch -M main
git push -u origin main
```

## 步骤 4：启用 GitHub Pages
1. 进入仓库 Settings → Pages
2. Source 选择 `main` 分支
3. 保存后等待几分钟
4. 访问地址：`https://你的用户名.github.io/competitor-analysis/`

---

## 或者：使用 Vercel 一键部署（更简单）
```bash
cd c:\cyz\工作文档\陈远卓\Python\article\LSTM_Stock-main\LSTM_Stock
npx vercel deploy --prod
```
首次使用会要求登录，按提示操作即可。部署完成后会获得一个 `xxx.vercel.app` 的公网地址。
