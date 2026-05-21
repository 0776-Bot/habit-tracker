# 打卡 · 个性化习惯计划生成器

一个给朋友的小工具。和 AI 聊几分钟,生成一份属于你自己的 12 周打卡计划,在网页上每天打卡。

## 文件结构

```
site/
├── index.html              # 首页(介绍 + 怎么用 + 4 个示例)
├── tracker.html            # 打卡追踪器
├── habit-plan-skill.md     # AI skill 内容(首页会读取并显示)
├── examples/               # 示例计划文件
│   ├── ielts-6-5.md
│   ├── fitness-fat-loss.md
│   ├── cooking-30-dishes.md
│   └── reading-writing-habit.md
└── README.md               # 这个文件
```

## 部署到 GitHub Pages

### 步骤 1: 建 GitHub 仓库

1. 登录 [github.com](https://github.com)
2. 点右上 **+** → **New repository**
3. 仓库名:任意,比如 `habit-tracker`
4. 选 **Public**(免费版要求)
5. 勾上 **Add a README file**
6. 点 **Create repository**

### 步骤 2: 上传文件

最简单的方式:在仓库页面点 **Add file** → **Upload files**,把整个 `site/` 文件夹里的所有文件拖进去(注意是文件,不是文件夹本身)。

或者用命令行:

```bash
git clone https://github.com/你的用户名/habit-tracker.git
cd habit-tracker
# 把 site/ 里所有文件复制到这个目录
cp -r /path/to/site/* .
git add .
git commit -m "Initial commit"
git push
```

### 步骤 3: 开启 GitHub Pages

1. 仓库页面 → **Settings**
2. 左侧菜单 → **Pages**
3. **Source** 选 `Deploy from a branch`
4. **Branch** 选 `main` 和 `/(root)`
5. 点 **Save**
6. 等 1-2 分钟,顶部会显示你的网址,类似:

```
https://你的用户名.github.io/habit-tracker/
```

### 步骤 4: 测试

打开这个网址,你应该看到:
- 首页正常显示
- "怎么用"那里的 skill 内容能加载出来
- 4 个示例卡片能下载 .md
- 点"打开追踪器"能进入 tracker.html
- 追踪器的"导入计划"能加载示例 .md 文件

如果某步出问题,常见原因:
- skill 加载不出来 → 检查 `habit-plan-skill.md` 是否和 `index.html` 在同一目录
- 示例下载不了 → 检查 `examples/` 文件夹是否正确上传
- 追踪器报错 → 看浏览器控制台(F12)

### 步骤 5: 发给朋友

把这个网址复制到微信发给朋友。建议附一句话:

> 这个小工具帮你做个性化打卡计划,聊几分钟就能开始。三步:
> 1. 复制 skill 到你常用的 AI
> 2. 聊完保存 .md 文件
> 3. 导入到追踪器开始打卡

## 修改和定制

### 改首页文案

直接编辑 `index.html`。所有文案都是中文,在 `<body>` 标签内可以找到。

### 改默认配色

`index.html` 顶部 `<style>` 里的 CSS 变量:

```css
--bg: #faf7f2;          /* 背景色 */
--ink: #2a2419;          /* 主文字色 */
--accent: #b8420f;       /* 强调色 */
```

### 加新示例

1. 在 `examples/` 文件夹里加新的 `.md` 文件(格式参考现有 4 个)
2. 在 `index.html` 的 `.examples-grid` 里加一个新的 `.example-card`

### 改默认 CONFIG

`tracker.html` 顶部的 `DEFAULT_CONFIG` 对象——这是用户没导入任何计划时看到的内容。

## 隐私和数据

- 所有打卡数据存在用户自己的浏览器 localStorage 里
- 你(仓库所有者)看不到任何用户数据
- 用户清浏览器缓存数据会丢 — 追踪器内置了"备份打卡"按钮可以导出 JSON
- 这是个**静态网站**,没有后端,所以没有用户系统、没有云存储

## 反馈

朋友用了之后想给你反馈,可以让他们:
- 发微信给你
- 在仓库提 Issue(如果他们有 GitHub 账号)

你看到反馈后,改 HTML/skill 文件,push 到仓库,GitHub Pages 会自动更新。
