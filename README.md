# 火柴人影子战士 · Android 应用

通过 **GitHub Actions 自动打包 APK**，不是网站。

## 下载 APK（应用安装包）

1. 打开：https://github.com/yxing7249-cmd/n/actions
2. 点开最新一次 **Build Android APK** 成功的运行
3. 页面底部 **Artifacts** 里下载 `stickman-shadow-warrior-apk`
4. 解压得到 `.apk`，传到手机/安卓电视安装

也可以在 Actions 页点 **Run workflow** 手动触发构建。

## 本地打包（可选）

```bash
npm install
npx cap add android
npx cap sync android
npx cap open android
```

## License

MIT
