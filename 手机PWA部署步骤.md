# GrowthOS PRD 手机 PWA 部署步骤

## 第一步：把文件拿到你的电脑

1. 在 Trae 中，找到左侧文件栏里的 `growthos-prd` 文件夹
2. 右键点击 `growthos-prd` 文件夹 → **下载**（或导出到本地）
3. 解压后你会得到一个文件夹，里面包含这些文件：
   ```
   growthos-prd/
   ├── index.html          # 入口文件
   ├── growthos-prd.html   # 原始文档
   ├── manifest.json       # PWA 配置
   ├── sw.js               # 离线缓存
   ├── icon.svg            # 应用图标
   ├── README.md           # 部署指南
   └── _shared/js/         # JS 依赖库
   ```

---

## 第二步：上传到 GitHub（免费部署）

### 2.1 注册 GitHub
- 手机或电脑浏览器打开 https://github.com
- 点击 **Sign up** 注册账号（用邮箱即可，免费）

### 2.2 创建仓库
1. 登录后，点击右上角 **+** 号 → **New repository**
2. **Repository name** 填写：`growthos-prd`
3. 下方选择 **Public**（公开）
4. 点击最下面的 **Create repository**

### 2.3 上传文件
1. 在新页面中，点击 **uploading an existing file**
2. 打开电脑上的 `growthos-prd` 文件夹
3. 把文件夹里的**所有文件和文件夹**拖入网页上传区域：
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon.svg`
   - `_shared/` 文件夹（里面有两个 js 文件）
4. 页面下方点击 **Commit changes**

### 2.4 开启网站访问
1. 仓库页面点击顶部的 **Settings**（设置）
2. 左侧菜单往下滑，点击 **Pages**
3. **Source** 下面选择 **Deploy from a branch**
4. **Branch** 选择 **main** → 后面选 **/(root)**
5. 点击 **Save**
6. 等待 1-2 分钟，页面上方会出现绿色提示：
   ```
   Your site is live at https://你的用户名.github.io/growthos-prd/
   ```
7. 复制这个链接

---

## 第三步：手机添加到主屏幕

### iPhone（Safari）
1. 打开 Safari，粘贴访问链接
2. 等页面加载完成后，点击底部中间的 **分享按钮**（方框带箭头）
3. 上滑找到 **"添加到主屏幕"**
4. 点击 **添加**
5. 返回桌面，会出现 "GrowthOS" 图标，点击即可全屏打开

### 安卓手机（Chrome）
1. 打开 Chrome，粘贴访问链接
2. 等页面加载完成后，点击右上角 **三个点菜单**
3. 点击 **"安装应用"** 或 **"添加到主屏幕"**
4. 按提示确认
5. 返回桌面，会出现 "GrowthOS" 图标，点击即可全屏打开

---

## 完成效果

- 手机桌面有独立图标
- 点击后全屏打开，没有浏览器地址栏
- 离线也能查看（只要之前打开过一次）
- 体验接近原生 App

---

## 常见问题

**Q：链接打不开？**  
A：GitHub Pages 在国内偶尔不稳定，等 2-3 分钟再试，或换 Vercel 方案。

**Q：怎么更新内容？**  
A：修改文件后重新上传到 GitHub 同一仓库，覆盖原文件，等待 1-2 分钟自动更新。

**Q：图标不显示？**  
A：清除手机浏览器缓存，或删除主屏幕图标重新添加。
