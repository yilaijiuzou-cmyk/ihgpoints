# 部署到 GitCode Pages

## 一次性操作

```bash
# 1. 在 docs/ 目录下初始化 git
cd D:/life/line/docs

git init
git add index.html manifest.json icon.svg sw.js GITCODE_DEPLOY.md
git commit -m "init: IHG积分购买价值评估工具 v2.0 移动优化版"

# 2. 添加远程仓库
git remote add origin https://gitcode.net/yilaijiuzou/ihg-points-value.git

# 3. 推送
git push -u origin master
```

## 在 GitCode 网站上开启 Pages

1. 打开 https://gitcode.net/yilaijiuzou/ihg-points-value
2. 进入 **设置 → Pages**
3. 部署来源：选择 **master 分支**
4. 目录：**/**（根目录）
5. 点击 **保存**

## 完成

等待 1~2 分钟，访问：

```
https://yilaijiuzou.gitcode.io/ihg-points-value/
```

## 后续更新

修改文件后：

```bash
git add -A
git commit -m "更新说明"
git push
```

GitCode Pages 会自动同步更新（等待 1~2 分钟生效）。

## PWA 提示

- **Android Chrome**：访问链接后，底部会弹出「添加到主屏幕」，点击后生成 App 图标
- **iPhone Safari**：用 Safari 打开 → 底部分享按钮 → 「添加到主屏幕」
- 添加后，图标会显示在桌面，点开全屏运行，无地址栏
