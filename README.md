# 骆子谦 - 在线简历

HTML + Tailwind CSS 制作的个人简历，支持在线浏览和 PDF 导出。

## 在线预览

**[https://luoziqianx.github.io/resume/](https://luoziqianx.github.io/resume/)**

## 文件结构

```
├── index.html       # 简历页面（Tailwind CSS via CDN）
├── photo.jpg        # 证件照
├── 骆子谦_简历.pdf   # PDF 导出版本
└── README.md
```

## 技术栈

- **布局**：双栏（深色侧边栏 + 白色主内容区）
- **样式**：[Tailwind CSS](https://tailwindcss.com/) CDN + 自定义 print CSS
- **字体**：[Inter](https://fonts.google.com/specimen/Inter) + [Noto Sans SC](https://fonts.google.com/noto/specimen/Noto+Sans+SC)
- **图标**：[Font Awesome 6](https://fontawesome.com/)

## PDF 导出

使用 Chrome 无头模式导出单页 A4 PDF：

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless=new --disable-gpu --no-pdf-header-footer \
  --virtual-time-budget=5000 \
  --print-to-pdf=骆子谦_简历.pdf \
  file://$(pwd)/index.html
```

## 联系方式

- **Email**: luoziqian1400961546@outlook.com
- **GitHub**: [luoziqianX](https://github.com/luoziqianX)
- **Kaggle**: [luoziqian](https://www.kaggle.com/luoziqian)
