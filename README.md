# 毕设源码大全 - GitHub Pages 展示站

## 部署到 GitHub Pages 步骤

### 1. 创建 GitHub 仓库

1. 登录 GitHub
2. 新建仓库，名称建议：`你的用户名.github.io`（这样可以直接用根域名访问）
   - 或者用任意名称，比如 `bishe-site`，后面通过 Settings 开启 Pages

### 2. 上传文件

把这个目录下的所有文件上传到仓库：
```
index.html
projects.html
project-detail.html
topics.html
templates.html
about.html
assets/
```

### 3. 开启 GitHub Pages

1. 进入仓库的 `Settings`
2. 左侧菜单找到 `Pages`
3. Source 选择 `Deploy from a branch`
4. Branch 选择 `main` 分支，目录选 `/root`
5. 点击 Save

### 4. 访问网站

等待1-2分钟，访问：
- 如果仓库名是 `你的用户名.github.io`：https://你的用户名.github.io
- 如果仓库名是 `bishe-site`：https://你的用户名.github.io/bishe-site/

---

## 自定义域名（可选）

如果有自己的域名：
1. 在仓库根目录创建 `CNAME` 文件，内容写你的域名，比如 `bisheku.com`
2. 在域名服务商那里添加 CNAME 记录，指向 `你的用户名.github.io`

---

## 内容更新

### 添加新项目

1. 编辑 `project-detail.html` 里的 `projects` 对象，添加新项目数据
2. 编辑 `projects.html`，添加新的项目卡片
3. 编辑 `index.html`，首页热门项目区添加卡片

### 修改联系方式

搜索所有文件中的 `bishe_helper`，替换成你的微信号。

### 替换微信二维码

在 `about.html` 中找到二维码位置，替换成你的真实二维码图片。

---

## 推荐配合使用

- GitHub 仓库：`computer-bishe-collection`（源码合集）
- GitHub Pages：这个展示站
- 独立网站：后续可以部署到国内服务器，做百度SEO
