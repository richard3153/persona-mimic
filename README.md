# persona-mimic / 人格预设库

> AI Character Persona Database — 收录1000位世界名人，涵盖科学家、企业家、艺术家等8大领域

---

## 简介 | Introduction

**persona-mimic** 是一个大型AI角色人格预设数据库，收录了 **1000位** 来自全球各领域的知名人物。同类角色预设包含丰富且一致的信息：
- **core** — 核心身份与定位
- **thinking** — 思维方式/认知模式
- **speaking** — 说话风格与表达特点
- **solving** — 解决问题的风格
- **quotes** — 经典语录/名言
- **recommended_skills** — 推荐技能标签（用于AI工具匹配）

适用于：
- AI角色扮演对话系统
- 大语言模型(LLM)的few-shot prompting
- 创意写作与故事创作
- 学科教学人物模拟
- 游戏NPC性格设计

---

## 数据结构 | Contents

```
characters/
├── 01_scientists.json      科学家与发明家 (160人)
├── 02_artists.json        艺术家与音乐家 (55人)
├── 03_entrepreneurs.json  企业家与商业领袖 (133人)
├── 04_athletes.json       运动员 (246人)
├── 05_writers.json         作家与思想家 (90人)
├── 06_actors.json          演员与导演 (124人)
├── 07_historical.json      历史人物 (66人)
└── 08_others.json          其他领域名人 (126人)
        Total: 1000人
```

---

## 快速开始 | Quick Start

### 安装方式一：SkillHub CLI（推荐）
```bash
skillhub install persona-mimic
```

### 安装方式二：GitHub 直链
```bash
git clone https://github.com/richard3153/persona-mimic.git
```

### 安装方式三：直接下载 JSON
下载任意角色文件：
```
https://raw.githubusercontent.com/richard3153/persona-mimic/main/characters/01_scientists.json
https://raw.githubusercontent.com/richard3153/persona-mimic/main/characters/02_artists.json
...
https://raw.githubusercontent.com/richard3153/persona-mimic/main/characters/08_others.json
```

### 安装方式四：Release 包
下载 [v1.0.0 Release](https://github.com/richard3153/persona-mimic/releases/tag/v1.0.0) 完整压缩包（无需 SkillHub）。

---

## 人物示例 | Character Examples

| 领域 | 角色 | 核心定位 | 思维方式 |
|------|------|----------|----------|
| 科学 | 爱因斯坦 | 相对论创立者 | 第一性原理直觉 |
| 商业 | 埃隆·马斯克 | SpaceX/Tesla创始人 | 第一性原理思维 |
| 商业 | 乔布斯 | 苹果教主 | 细节完美主义者 |
| 体育 | 乔丹 | 篮球GOAT | 赢家心态 |
| 演员 | 周星驰 | 喜剧之王 | 无厘头喜剧天才 |
| 科学 | 图灵 | 计算机科学之父 | 跨学科天才 |
| 导演 | 诺兰 | 烧脑导演 | 烧脑逻辑派 |
| 历史 | 成吉思汗 | 蒙古帝国建立者 | 征服与恐惧 |

---

## 技能标签 | Skill Tags

| 标签 | 说明 | 数量 |
|------|------|------|
| athlete_basketball | 篮球运动员 | 133 |
| musician_pop | 流行歌手 | 125 |
| actor_classical | 演员 | 106 |
| entrepreneur_tech | 科技企业家 | 65 |
| athlete_soccer | 足球运动员 | 49 |
| scientist_ai | AI/计算机科学家 | 94 |
| business_ceo | CEO/企业高管 | 47 |
| writer | 作家 | 38 |
| director | 导演 | 37 |
| scientist_physics | 物理学家 | 30 |
| philosopher_western | 西方哲学家 | 17 |
| entrepreneur_chinese | 中国企业家 | 16 |
| athlete_chinese | 中国运动员 | 18 |
| military_commander | 军事指挥官 | 10 |
| activist | 社会活动家 | 4 |

共 **45种** 技能标签，精准覆盖全部1000位人物。

---

## 数据格式 | Data Format

```json
{
  "id": "albert_einstein",
  "name": "Albert Einstein",
  "zhName": "阿尔伯特·爱因斯坦",
  "years": "1879-1955",
  "field": "物理学",
  "core": "相对论创立者，现代物理学奠基人",
  "thinking": "第一性原理思维与物理直觉",
  "speaking": "睿智、幽默、反权威",
  "solving": "思想实验与数学推导结合",
  "quotes": ["想象力比知识更重要", "上帝不掷骰子"],
  "recommended_skills": ["scientist_physics", "online-search"]
}
```

---

## 使用场景 | Use Cases

### AI角色扮演
```
用户：请以爱因斯坦的思维方式，回答什么是相对论。
AI：[扮演爱因斯坦] 想象你正坐在一束光上...
```

### Few-shot Prompting
```
系统：作为一个[角色]专家，具备[思维方式]，擅长...
```

### 创意写作
```
请写一个马斯克创办火星公司的商业故事。
```

### 游戏NPC性格
```
一个性格像乔布斯的游戏NPC，柜台老板要追求完美。
```

---

## OpenClaw 安装 | OpenClaw Installation

```bash
# 方式一：SkillHub（推荐）
skillhub install persona-mimic

# 方式二：手动安装
cp -r characters/ /path/to/openclaw/config/skills/persona-mimic/
cp SKILL.md /path/to/openclaw/config/skills/persona-mimic/
```

---

## 贡献 | Contributing

欢迎提交PR，拓展更多人物！

---

## 许可证 | License

MIT License

---

⭐ If helpful, please give it a star!
