## Hi there 👋

<!--
**ZhYQ1/ZhYQ1** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->



---

## GitHub Actions / Community Actions

### 🌍 github-gravity

GitHub Gravity 让你的 GitHub 贡献图在引力作用下落下，并与自定义文本发生碰撞，生成漂亮的动画 SVG。

**功能：**
- 🎮 交互式重力动画：贡献方块落下并撞击自定义文字
- 🌈 支持自定义文字、字体、背景色、文本颜色
- 🟢 圆形或方形贡献块
- 🎚️ 可调节摩擦力、弹性、缩放、播放速度、物理世界尺寸
- 🎨 支持 CSS 或 SMIL 动画引擎
- 📦 自动压缩轨迹、减小 SVG 文件体积

**输入参数：**
- `username`：GitHub 用户名（必填）
- `text`：要在画面中作为碰撞障碍物的文字
- `output-path`：生成 SVG 的路径
- `font-size`：文字字体大小，默认 48
- `compression-tolerance`：轨迹压缩容忍度，默认 0.5
- `compression-algorithm`：压缩算法，默认 Greedy
- `max-simulation-time`：最大模拟时长
- `shape`：贡献块形状，circle 或 square
- `friction`：摩擦系数，默认 0.3
- `restitution`：弹性系数，默认 0
- `text-top`：文字距顶部距离，默认 50
- `background-color`：SVG 背景色，默认 transparent
- `text-color`：文字颜色，默认 black
- `scale`：整体缩放倍数，默认 3
- `speed`：播放速度倍数，默认 3
- `css`：是否使用 CSS 动画引擎，默认 false
- `width`：物理世界宽度，默认 300
- `height`：物理世界高度，默认 150
- `size`：贡献块边长，默认 4
- `interval`：贡献块间距，默认 1.5
- `font-path`：自定义字体文件路径或 URL

**使用示例：**

```yaml
- name: Generate Gravity SVG
  uses: flycran/github-gravity@v1
  with:
    username: ZhYQ1
    text: GitHub Gravity
    output-path: gravity.svg
```

你也可以查看完整参数文档：  
https://github.com/marketplace/actions/github-gravity

---

### 📦 pacman-profile-github

PACMAN Profile GitHub 把你的 GitHub/GitLab 贡献图变成一个互动的 Pac-Man 游戏，带 12 种配色主题和多平台支持。

**功能：**
- 🎮 互动游戏：在贡献日历上玩 Pac-Man
- 🎨 12 种颜色主题：6 个主题族 × 2 种浅色/深色变体
  - GitHub
  - GitLab
  - React
  - Dracula
  - Solarized
  - Monokai
- 📊 支持 GitHub、GitLab 等平台
- 🎵 可选的经典 Pac-Man 音效
- 🚀 高性能：优化后的 canvas/SVG 渲染
- 📦 支持 NPM 包、CLI 工具或 GitHub Action
- ⚡ 自动浅色/深色模式检测
- ⏱️ 支持周期性生成 SVG，自动推送到输出分支

**使用示例：**

```yaml
- name: Generate Pac-Man Graph
  uses: DuyetBKU/viz-pacman-github-profile@main
  with:
    github_user_name: ZhYQ1
    github_token: ${{ secrets.GITHUB_TOKEN }}
    theme: react-dark
    music: 'false'
```

**README 中展示贡献图：**

```html
<div align="center">
	<h2>📊 My Contribution Activity</h2>

	<picture>
		<source
			media="(prefers-color-scheme: dark)"
			srcset="
				https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/dist/pacman-contribution-graph-dark.svg
			"
		/>
		<source
			media="(prefers-color-scheme: light)"
			srcset="
				https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/dist/pacman-contribution-graph-light.svg
			"
		/>
		<img
			alt="Pacman Contribution Graph"
			src="https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/dist/pacman-contribution-graph-light.svg"
		/>
	</picture>
</div>
```

你也可以查看完整主题和使用指南：  
https://github.com/marketplace/actions/pacman-profile-github

---


---

## GitHub Actions / Community Actions

### 🌍 github-gravity

GitHub Gravity 让你的 GitHub 贡献图在引力作用下落下，并与自定义文本发生碰撞，生成漂亮的动画 SVG。

**功能：**
- 🎮 交互式重力动画：贡献方块落下并撞击自定义文字
- 🌈 支持自定义文字、字体、背景色、文本颜色
- 🟢 圆形或方形贡献块
- 🎚️ 可调节摩擦力、弹性、缩放、播放速度、物理世界尺寸
- 🎨 支持 CSS 或 SMIL 动画引擎
- 📦 自动压缩轨迹、减小 SVG 文件体积

**输入参数：**
- `username`：GitHub 用户名（必填）
- `text`：要在画面中作为碰撞障碍物的文字
- `output-path`：生成 SVG 的路径
- `font-size`：文字字体大小，默认 48
- `compression-tolerance`：轨迹压缩容忍度，默认 0.5
- `compression-algorithm`：压缩算法，默认 Greedy
- `max-simulation-time`：最大模拟时长
- `shape`：贡献块形状，circle 或 square
- `friction`：摩擦系数，默认 0.3
- `restitution`：弹性系数，默认 0
- `text-top`：文字距顶部距离，默认 50
- `background-color`：SVG 背景色，默认 transparent
- `text-color`：文字颜色，默认 black
- `scale`：整体缩放倍数，默认 3
- `speed`：播放速度倍数，默认 3
- `css`：是否使用 CSS 动画引擎，默认 false
- `width`：物理世界宽度，默认 300
- `height`：物理世界高度，默认 150
- `size`：贡献块边长，默认 4
- `interval`：贡献块间距，默认 1.5
- `font-path`：自定义字体文件路径或 URL

**使用示例：**

```yaml
- name: Generate Gravity SVG
  uses: flycran/github-gravity@v1
  with:
    username: ZhYQ1
    text: GitHub Gravity
    output-path: gravity.svg
```

你也可以查看完整参数文档：  
https://github.com/marketplace/actions/github-gravity

---

### 📦 pacman-profile-github

PACMAN Profile GitHub 把你的 GitHub/GitLab 贡献图变成一个互动的 Pac-Man 游戏，带 12 种配色主题和多平台支持。

**功能：**
- 🎮 互动游戏：在贡献日历上玩 Pac-Man
- 🎨 12 种颜色主题：6 个主题族 × 2 种浅色/深色变体
  - GitHub
  - GitLab
  - React
  - Dracula
  - Solarized
  - Monokai
- 📊 支持 GitHub、GitLab 等平台
- 🎵 可选的经典 Pac-Man 音效
- 🚀 高性能：优化后的 canvas/SVG 渲染
- 📦 支持 NPM 包、CLI 工具或 GitHub Action
- ⚡ 自动浅色/深色模式检测
- ⏱️ 支持周期性生成 SVG，自动推送到输出分支

**使用示例：**

```yaml
- name: Generate Pac-Man Graph
  uses: DuyetBKU/viz-pacman-github-profile@main
  with:
    github_user_name: ZhYQ1
    github_token: ${{ secrets.GITHUB_TOKEN }}
    theme: react-dark
    music: 'false'
```

**README 中展示贡献图：**

```html
<div align="center">
	<h2>📊 My Contribution Activity</h2>

	<picture>
		<source
			media="(prefers-color-scheme: dark)"
			srcset="
				https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/dist/pacman-contribution-graph-dark.svg
			"
		/>
		<source
			media="(prefers-color-scheme: light)"
			srcset="
				https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/dist/pacman-contribution-graph-light.svg
			"
		/>
		<img
			alt="Pacman Contribution Graph"
			src="https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/dist/pacman-contribution-graph-light.svg"
		/>
	</picture>
</div>
```

你也可以查看完整主题和使用指南：  
https://github.com/marketplace/actions/pacman-profile-github

![snake](https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/github-snake-dark.svg#gh-dark-mode-only)


---

## GitHub Actions / Community Actions

- 🌍 [github-gravity](https://github.com/marketplace/actions/github-gravity) — 一个 GitHub Marketplace 上的 Action，可用于将仓库/账号相关信息以更易读的方式展示出来。
- 📦 [pacman-profile-github](https://github.com/marketplace/actions/pacman-profile-github) — 一个 GitHub Marketplace 上的 Action，可用于将 Pacman/Arch Linux 相关配置或个人资料信息以 GitHub 友好的方式展示。

![snake](https://raw.githubusercontent.com/ZhYQ1/ZhYQ1/output/github-snake-dark.svg#gh-dark-mode-only)
