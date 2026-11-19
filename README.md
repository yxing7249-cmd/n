# 火柴人影子战士 · 应用版

可安装的火柴人横版动作游戏（电视 / 手机 / 平板）。

支持两种形态：
1. **PWA 应用** — 浏览器打开后「添加到主屏幕」即可安装
2. **Android APK** — 用 Capacitor 打包成真正的安卓应用（含 Android TV）

---

## 一、作为 PWA 安装（最简单）

1. 用手机或电脑浏览器打开 `www/index.html`（或部署到网站）
2. 浏览器菜单选择 **「添加到主屏幕」/「安装应用」**
3. 图标会出现在桌面，全屏运行，像原生应用一样

本地预览：
```bash
cd stickman-shadow-warrior-app
npm start
# 浏览器打开 http://localhost:3000
```

开启 GitHub Pages 后可访问：
`https://yxing7249-cmd.github.io/n/`

---

## 二、打包成 Android APK

### 环境要求
- Node.js 18+
- Android Studio（含 SDK）
- JDK 17

### 步骤

```bash
cd stickman-shadow-warrior-app   # 或本仓库根目录
npm install
npx cap add android
npx cap sync android
npx cap open android
```

在 Android Studio 中：**Build → Build APK(s)**  
APK 一般在：`android/app/build/outputs/apk/debug/app-debug.apk`

---

## 三、项目结构

```
www/                 # 游戏 + PWA
  index.html
  manifest.json
  sw.js
  icons/
capacitor.config.json
package.json
LICENSE
README.md
```

## 四、操作

| 输入 | 操作 |
|------|------|
| 方向键 / 虚拟键 | 移动、跳跃 |
| 确认 / 攻击键 | 轻攻击、菜单确认、必杀 |
| 下键 / 重击 | 重攻击 |
| 双击左右 | 冲刺 |

5 名角色各有专属技能，见游戏内角色选择界面。

## License

MIT
