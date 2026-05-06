# 立方舟 — 药膳官网

> 传承中医智慧，品味健康生活

## 项目简介

立方舟药膳官网是一个展示型网站，致力于推广药膳文化，提供药膳商品展示、一对一中医诊疗预约、以及中医药学术文献阅读等服务。网站融合了传统中医元素与现代 Web 技术，为用户带来独特的浏览体验。

## 技术架构

### 核心技术栈

| 技术 | 说明 |
|------|------|
| **HTML5 + CSS3** | 语义化标签与现代化 CSS |
| **JavaScript** | 原生 JavaScript，无框架依赖 |
| **Bootstrap 5.3.0** | UI 框架，响应式栅格系统 |
| **Less** | CSS 预处理器 |
| **Lenis** | 平滑滚动库 |

### 设计资源

- **图标**: iconfont 字体图标库
- **框架**: Bootstrap 5.3.0-alpha1

## 功能模块

### 1. 导航栏
- 响应式折叠菜单（移动端）
- Logo 点击返回首页
- 移动端显示通知小红点

### 2. 轮播横幅
- 自动轮播宣传图片
- 手动切换与指示器导航

### 3. 推荐产品

| 产品名称 | 功效 |
|----------|------|
| 艾草根炖乌鸡 | 散寒、温中益气 |
| 乳鸽汤 | 利水渗湿，健脾和胃 |
| 参桂酒 | 补气益虚，温通经脉 |
| 鸟不企药酒 | 祛风除湿，活血通经 |

### 4. 中医药文化
- PC 端：横版大图布局
- 移动端：自适应竖版
- 链接到 PDF 文献页面

### 5. 新闻与活动
- 活动卡片展示
- 学术文献列表

### 6. 其他页面
- **商品页**: 商品展示网格与筛选
- **诊疗页**: 一对一诊疗预约
- **PDF 文献页**: 学术文献阅读

## 目录结构

```
lifangzhou-official-website/
├── index.html                      # 首页
├── favicon.ico                     # 网站图标
├── bootstrap-5.3.0-alpha1-dist/   # Bootstrap 库
├── css/                            # 样式文件
│   ├── base.css
│   ├── normalize.css
│   ├── common.css
│   ├── index.css
│   ├── chat.css
│   ├── goods.css
│   └── pdf.css
├── iconfont/                       # 字体图标
├── img/                            # 图片资源
├── js/                             # 脚本文件
├── less/                           # Less 源文件
└── html/                           # 子页面
    ├── goods.html
    ├── chat.html
    └── pdf-page/                   # PDF 文献目录
```

## 开发指南

### 环境要求

直接用浏览器打开 `index.html` 即可预览。

### 使用本地服务器

```bash
python -m http.server 8000
npx serve .
php -S localhost:8000
```

### Less 编译

```bash
npm install -g less
lessc less/index.less css/index.css
```

## 浏览器兼容性

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## 版权信息

```
copyright © 立方舟 developed by Jason Liu
```

## 作者

- **GitHub**: [bigmanBass666](https://github.com/bigmanBass666)
- **Gitee**: [paeonia-lactiflora](https://gitee.com/paeonia-lactiflora)

---

**声明**: 本网站为学习和演示项目，部分产品和学术文献资料来自互联网，仅供学习参考使用。
