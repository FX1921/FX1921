# 星尘圣诞树 · 3D 手势互动网页

## 功能
- Three.js 3D 粒子圣诞树、螺旋粒子、发光星星、地面光环与环境星尘
- 鼠标/触摸拖动旋转；点击或按钮触发粒子扩散/聚合
- MediaPipe 手部关键点摄像头识别：张手扩散、握拳聚合、手掌左右移动旋转
- 手机/桌面响应式布局

## 运行
摄像头权限要求安全上下文 (HTTPS 或 localhost)。建议部署到 HTTPS 静态托管服务，或本地运行：

```bash
python -m http.server 8000
```

然后访问 `http://localhost:8000`。手机访问电脑的局域网 IP 通常不属于安全上下文，摄像头可能被浏览器阻止；手机端请部署 HTTPS。

本项目通过 CDN 加载 Three.js 和 MediaPipe Tasks Vision，首次使用需要联网。