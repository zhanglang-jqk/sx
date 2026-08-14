# 智能镜 · LVGL UI

智能镜（Smart Mirror）界面，**LVGL Pro** 项目，LVGL 9.5.0，1280×800。

## 项目结构

```
├── project.xml          ← LVGL 版本 + 1280×800 display
├── globals.xml          ← 配色常量 + 中文字体（MiSans）+ 全局样式
├── fonts/MiSans.ttf     ← 中文字体（小米 MiSans，免费商用）
└── screens/
    ├── home.xml         ← 主界面（状态栏/简报/卡片墙/小美助手）
    ├── face.xml         ← 面部会诊（扫描/指标/建议）
    └── settings.xml     ← 设置（网络/显示/语音/隐私/关于）
```

## 在线预览

本仓库为 **GitHub 公开仓库**，在 [viewer.lvgl.io](https://viewer.lvgl.io) 粘贴仓库 URL 即可加载预览（需 GitHub 登录）。

## 屏幕说明

| 屏幕 | 内容 |
|---|---|
| home | 顶部状态栏（时间/天气/路况/电量）、滚动简报条、7 张卡片（音乐/K歌/面部/皮肤/天气/日程/资讯）、小美同学助手栏 |
| face | AppBar、面部扫描预览、二级 Tab、7 项健康指标条、会诊建议、重新检测 |
| settings | 双栏设置组：网络与连接 / 显示与声音 / 语音助手 / 隐私与健康 / 关于 |

## 说明

- 界面还原自 HTML 设计稿（home-v3.html / apps-v1.html）。
- 毛玻璃/复杂渐变/SVG 图标等用 LVGL 能力近似（半透明、线性渐变、符号文字）。
- 中文字体 MiSans 需要 `fonts/` 目录存在，否则中文不显示。
- 数字/时间用 Outfit Thin（超细字重），还原 HTML 的 Outfit 200/300 设计。
