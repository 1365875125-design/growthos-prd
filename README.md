# GrowthOS PRD 部署指南

## 目录说明

```
growthos-prd/
├── index.html              # 主文档（入口文件）
├── growthos-prd.html       # 原始文档
├── _shared/js/             # JS 依赖库
│   ├── echarts.min.js      # 图表库
│   └── mermaid.min.js      # 流程图库
└── README.md               # 本文件
```

## 推荐方案：GitHub Pages（免费 + 永久在线）

### 步骤 1：注册/登录 GitHub
打开 https://github.com ，注册或登录账号。

### 步骤 2：创建新仓库
1. 点击右上角 **+** → **New repository**
2. 仓库名填写：`growthos-prd`
3. 选择 **Public**（公开）
4. 点击 **Create repository**

### 步骤 3：上传文件
1. 在新仓库页面，点击 **uploading an existing file**
2. 把本目录下所有文件和文件夹拖入上传区域（`index.html`、`_shared/`）
3. 点击 **Commit changes**

### 步骤 4：开启 GitHub Pages
1. 仓库页面点击 **Settings**（设置）
2. 左侧菜单点击 **Pages**
3. **Source** 选择 **Deploy from a branch**
4. **Branch** 选择 **main** → **/ (root)**
5. 点击 **Save**

### 步骤 5：访问链接
等待约 1-2 分钟后，访问：
```
https://你的用户名.github.io/growthos-prd/
```

手机浏览器打开这个链接即可查看。

---

## 备选方案 A：Vercel（国内访问较快）

1. 打开 https://vercel.com ，用 GitHub 账号登录
2. 点击 **Add New...** → **Project**
3. 选择 `growthos-prd` 仓库，点击 **Import**
4. Framework Preset 选择 **Other**
5. 点击 **Deploy**
6. 等待部署完成，获得 `https://xxxx.vercel.app` 链接

## 备选方案 B：腾讯云/阿里云对象存储

1. 购买对象存储服务（COS / OSS），费用约每月 1-5 元
2. 创建存储桶，开启「静态网站」功能
3. 上传本目录所有文件
4. 绑定自定义域名（可选）
5. 获得 HTTPS 访问链接

## 手机访问效果

文档已做移动端适配：
- 手机打开自动隐藏侧边导航
- 表格支持左右滑动
- 字体和间距自适应屏幕
- 流程图自动缩放

---

如有问题，可重新导出文档后按上述步骤操作。
