# liuzhou09.github.io

刘洲老师个人学术主页，基于 Jekyll 搭建，部署在 GitHub Pages。

## 快速开始

### 1. 克隆仓库

```bash
git clone https://github.com/lliuzhou09/liuzhou09.github.io.git
cd liuzhou09.github.io
```

### 2. 拉取最新代码

```bash
git pull origin main
```

### 3. 修改后提交并推送

```bash
git add -f _pages/about.md _data/navigation.yml
git commit -m "描述你改了什么"
git push origin main
```

> 注意：`_pages/` 和 `_data/` 在 `.gitignore` 中，需要 `-f` 强制添加。

---

## 如何修改页面内容

所有页面内容都在 `_pages/about.md` 文件中，导航栏在 `_data/navigation.yml`。

### Home（个人介绍）

在 `_pages/about.md` 中找到 `# Home` 段落，直接修改文字即可。

### Publications（论文）

找到 `# 📝 Publications` 部分：
- **Journal Papers**：在 `Selected Journal Papers` 列表中增删条目
- **Conference Papers**：在 `Selected Conference Papers` 列表中增删条目
- **Patents（专利）**：在 `Selected Chinese Patents` 列表中增删条目

### Honors & Awards（荣誉获奖）

找到 `# 🏆 Honors & Awards` 部分，每条格式：
```
- 2025年 奖项名称
```

### Membership（学术任职）

找到 `# 🏅 Membership` 部分，每条格式：
```
- 学会名称 职务
```

### Invited Talks（受邀报告）

找到 `# 🎤 Invited Talks` 部分，每条格式：
```
- [YYYY/MM/DD] "报告题目" —— 会议/机构名称，城市
```

### Reviewer（审稿）

找到 `# 🔍 Conference Reviewer / Area Chair` 部分，在 `Conferences:` 下增删会议名称。

### Teaching（教学）

找到 `# 📚 Teaching` 部分，每条格式：
```
- 课程名称, 学期
```

---

## 导航栏修改

编辑 `_data/navigation.yml`，格式如下：

```yaml
main:
  - title: "显示名称"
    url: "/#锚点id"
```

新增栏目需要在 `_pages/about.md` 中对应位置添加锚点：
```html
<span class='anchor' id='锚点id'></span>
```

---

## 本地预览（可选）

```bash
# 安装依赖
bundle install

# 启动本地服务
bundle exec jekyll serve
```

浏览器打开 `http://localhost:4000` 预览。
