# 立方舟 - 药膳官网

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
| **Magic Mouse** | 鼠标指针效果（可选） |

### 设计资源

- **图标**: iconfont 字体图标库
- **框架**: Bootstrap 5.3.0-alpha1
- **平滑滚动**: Lenis 1.0.45

## 功能模块

### 1. 导航栏

```
┌─────────────────────────────────────────────┐
│  [Logo] LIFANGZHOU  │ 药膳商品 │ 一对一诊疗 │ 关于我们 │
└─────────────────────────────────────────────┘
```

- 响应式折叠菜单（移动端）
- Logo 点击返回首页
- 移动端显示通知小红点

### 2. 轮播横幅

自动轮播的宣传图片：

| 序号 | 图片 | 用途 |
|------|------|------|
| 1 | banner4.png | 品牌宣传 |
| 2 | banner1.png | 产品展示 |

支持：
- 自动轮播
- 手动切换
- 指示器导航

### 3. 推荐产品

展示药膳产品卡片：

| 产品名称 | 功效 | 图片 |
|----------|------|------|
| 艾草根炖乌鸡 | 散寒、温中益气 | 外部图片 |
| 乳鸽汤 | 利水渗湿，健脾和胃，宁心安神 | rgt-new.png |
| 参桂酒 | 补气益虚，温通经脉 | sgj.png |
| 鸟不企药酒 | 祛风除湿，活血通经，解毒消肿 | nbq.png |

产品卡片特性：
- 悬停遮罩效果
- 产品分类标签
- 产品名称和功效
- "了解更多"按钮

### 4. 中医药文化

展示学术研究内容：

- PC 端：横版大图布局
- 移动端：自适应竖版
- 链接到 PDF 文献页面

### 5. 新闻与活动

#### 活动卡片 (col-md-4)
- 活动图片
- 活动标题
- 活动时间
- 活动描述

#### 文献列表
| 标题 | 日期 |
|------|------|
| 不同产地黄毛楤木根中齐墩果酸含量测定_刘军民 | 2024-04-24 |
| 从鸟不企中提取齐墩果酸工艺改进及含量测定 | 2024-04-24 |
| 黄毛楤木皂苷的抗衰老作用研究_裘名宜 | 2024-04-24 |
| 齐墩果酸的研究进展 | 2024-04-24 |
| 齐墩果酸对缺血性卒中的神经保护作用及机制研究进展 | 2024-04-24 |
| 齐墩果酸抗肿瘤作用及机制研究进展 | 2024-04-24 |
| 用正交实验法优选从鸟不企中提取齐墩果酸的工艺条件 | 2024-04-24 |

### 6. 其他页面

#### 商品页 (html/goods.html)
- 商品展示网格
- 商品筛选功能
- 商品详情展示

#### 诊疗页 (html/chat.html)
- 一对一诊疗预约
- 咨询表单

#### PDF 文献页 (html/pdf-page/*.html)
学术文献阅读页面：
- 不同产地黄毛楤木根中齐墩果酸含量测定
- 从鸟不企中提取齐墩果酸工艺改进及含量测定
- 黄毛楤木皂苷的抗衰老作用研究
- 齐墩果酸的研究进展
- 等等...

## 目录结构

```
lifangzhou-official-website/
├── index.html                      # 首页
├── favicon.ico                     # 网站图标
├── bootstrap-5.3.0-alpha1-dist/   # Bootstrap 库
│   ├── css/
│   │   ├── bootstrap.css          # 完整 Bootstrap
│   │   └── bootstrap.min.css      # 压缩版本
│   └── js/
│       ├── bootstrap.js            # Bootstrap JS
│       └── bootstrap.bundle.js     # 捆绑版本(含 Popper)
├── css/                            # 样式文件
│   ├── base.css                    # 基础样式
│   ├── normalize.css               # 样式重置
│   ├── common.css                  # 公共样式
│   ├── index.css                   # 首页样式
│   ├── chat.css                    # 诊疗页样式
│   ├── goods.css                   # 商品页样式
│   ├── pdf.css                     # PDF 阅读页样式
│   └── removeScrollbar.css         # 滚动条隐藏
├── iconfont/                       # 字体图标
│   └── iconfont.css
├── img/                            # 图片资源
│   ├── banner/                     # 轮播图片
│   │   ├── banner1.png
│   │   ├── banner2.png
│   │   ├── banner3.png
│   │   └── banner4.png
│   ├── herb/                       # 中药材图片
│   ├── product/                    # 产品图片
│   │   ├── nbq.png                 # 鸟不企
│   │   ├── rgt.png / rgt-new.png   # 乳鸽汤
│   │   ├── sgj.png                 # 参桂酒
│   │   └── wjt.png
│   ├── pdf-img/                    # PDF 文献封面
│   ├── result_pc.png              # PC 端结果图
│   ├── result_mb.png              # 移动端结果图
│   ├── logo.png                   # Logo
│   └── lilac.jpg                  # 装饰图片
├── js/                             # 脚本文件
│   ├── index.js                    # 首页逻辑
│   ├── chat.js                     # 诊疗页逻辑
│   ├── goods.js                    # 商品页逻辑
│   ├── flexible.js                 # 响应式适配
│   └── magic_mouse.js              # 鼠标效果
├── less/                           # Less 源文件
│   ├── common.less                 # 公共样式
│   ├── index.less                  # 首页样式
│   ├── goods.less                  # 商品页样式
│   └── pdf.less                    # PDF 页样式
└── html/                           # 子页面
    ├── goods.html                  # 商品页
    ├── chat.html                   # 一对一诊疗页
    ├── other.html                  # 其他页
    └── pdf-page/                    # PDF 文献目录
        ├── 不同产地黄毛楤木根中齐墩果酸含量测定_刘军民.html
        ├── 从鸟不企中提取齐墩果酸工艺改进及含量测定.html
        ├── 用正交实验法优选从鸟不企中提取齐墩果酸的工艺条件.html
        ├── 黄毛楤木不同部位中齐墩果酸含量测定.html
        ├── 黄毛楤木皂苷的抗衰老作用研究_裘名宜.html
        ├── 齐墩果酸对缺血性卒中的神经保护作用及机制研究进展.html
        ├── 齐墩果酸抗肿瘤作用及机制研究进展.html
        └── 齐墩果酸的研究进展.html
```

## CSS 架构

样式采用分层设计：

```
normalize.css → base.css → common.css → 页面特定样式
```

| 文件 | 作用 |
|------|------|
| normalize.css | 跨浏览器样式一致性 |
| base.css | CSS 变量和基础重置 |
| common.css | 公共组件样式 |
| index.css | 首页特定样式 |
| chat.css | 诊疗页样式 |
| goods.css | 商品页样式 |

## 特色功能

### Lenis 平滑滚动

```javascript
const lenis = new Lenis()

function raf(time) {
  lenis.raf(time)
  requestAnimationFrame(raf)
}

requestAnimationFrame(raf)
```

### Magic Mouse 效果（已注释）

可选的鼠标指针增强效果：

```javascript
document.querySelectorAll('a, button, .card, .recommendInfo .imgBox, .news .list-group-item')
  .forEach(el => {
    el.classList.add('magic-hover')
  })

const options = {
  "outerStyle": "disable",
  "hoverEffect": "pointer-overlay",
  "hoverItemMove": false,
  "defaultCursor": false,
  "outerWidth": 30,
  "outerHeight": 30
}
magicMouse(options)
```

### 响应式图片

使用 Bootstrap 的响应式图片类：

```html
<img class="img-fluid" src="..." alt="...">
```

## 开发指南

### 环境要求

无需特殊开发环境，直接用浏览器打开即可预览。

### 使用本地服务器

```bash
# Python
python -m http.server 8000

# Node.js
npx serve .

# PHP
php -S localhost:8000
```

### Less 编译

如需修改 Less 源文件：

```bash
# 安装 less
npm install -g less

# 编译
lessc less/index.less css/index.css
```

或使用 VSCode 的 Easy LESS 插件自动编译。

## 内容来源

### 产品图片

部分产品图片来自网络：
- 艾草根炖乌鸡：[凤凰网](https://d.ifengimg.com)

### 学术文献

PDF 文献来源包括：
- 刘军民等人的研究论文
- 裘名宜等人的研究成果
- 其他中医药学术研究

## 浏览器兼容性

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## 版权信息

```
copyright © 立方舟 developed by Jason Liu
```

## 联系方式

- **作者**: Jason Liu
- **Gitee**: [paeonia-lactiflora](https://gitee.com/paeonia-lactiflora)

---

**声明**: 本网站为学习和演示项目，部分产品和学术文献资料来自互联网，仅供学习参考使用。药膳产品图片等内容版权属于原作者。
