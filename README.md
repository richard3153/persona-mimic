# persona-mimic / 人格预设库

> AI Character Persona Database — 1000 Famous Historical & Contemporary Figures  
> AI人格预设数据库 — 收录1000位古今中外名人，涵盖科学、商业、艺术、体育等8大领域

---

## 简介 | Introduction

**persona-mimic** 是一个大型AI角色扮演数据库，收录了 **1000位** 来自全球各地、不同领域的名人。

每个人物预设包含丰富的维度信息：
- **core** — 核心身份与定位
- **thinking** — 思维方式与认知模式
- **speaking** — 说话风格与表达特点
- **solving** — 解决问题的方式
- **quotes** — 经典语录/名言
- **recommended_skills** — 推荐技能标签（用于AI工具匹配）

适合用于：
- AI角色扮演对话系统
- 大语言模型(LLM)的few-shot prompting
- 创意写作与故事创作
- 教学场景的人物模拟
- 游戏NPC性格设计

---

## 内容结构 | Contents

```
characters/
├── 01_scientists.json     科学家与发明家 (160人)
├── 02_artists.json        艺术家与音乐家 (55人)
├── 03_entrepreneurs.json  企业家与商业领袖 (133人)
├── 04_athletes.json       运动员 (246人)
├── 05_writers.json        作家与思想家 (90人)
├── 06_actors.json         演员与导演 (124人)
├── 07_historical.json      历史人物 (66人)
└── 08_others.json         其他领域名人 (126人)
```

---

## 快速开始 | Quick Start

### 安装方式一：SkillHub（推荐）
```bash
skillhub install persona-mimic
```

### 安装方式二：GitHub下载
```bash
git clone https://github.com/richard3153/persona-mimic.git
```

### 安装方式三：手动安装
将 `characters/` 目录和 `SKILL.md` 复制到OpenClaw技能目录。

---

## 人物示例 | Character Examples

| 领域 | 姓名 | 核心特质 | 思维方式 |
|------|------|----------|----------|
| 物理 | 爱因斯坦 | 相对论创立者 | 第一性原理与直觉 |
| 商业 | 埃隆·马斯克 | SpaceX/Tesla创始人 | 第一性原理与垂直整合 |
| 篮球 | 迈克尔·乔丹 | 篮球之神 | 竞争与细节极致 |
| 足球 | 梅西 | 足坛GOAT | 天赋与团队 |
| 艺术 | 宫崎骏 | 动画大师 | 想象力与人文关怀 |
| 哲学 | 尼采 | 存在主义哲学家 | 批判与超人哲学 |
| 演员 | 周星驰 | 喜剧之王 | 无厘头与草根共鸣 |
| 历史 | 拿破仑 | 法国皇帝 | 野心与军事天才 |

---

## 技能标签 | Skill Tags

| 标签 | 说明 | 人数 |
|------|------|------|
| athlete_basketball | 篮球运动员 | 133 |
| musician_pop | 流行音乐人 | 125 |
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

共 **45种技能标签**，覆盖全部1000位人物。

---

## 数据格式 | Data Format

```json
{
  "id": "albert_einstein",
  "name": "Albert Einstein",
  "zhName": "阿尔伯特·爱因斯坦",
  "years": "1879-1955",
  "field": "物理学",
  "core": "相对论创立者，现代物理学的奠基人",
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
用户：扮演爱因斯坦，用他的思维方式和我讨论量子力学
AI：根据爱因斯坦的思维模式（第一性原理、反权威）...
```

### Few-shot Prompting
```
系统提示：作为一个[领域]专家，你以[思维方式]著称...
```

### 创意写作
```
帮我写一段乔布斯在产品发布会上的演讲
```

### 教学模拟
```
扮演苏格拉底，用问答法讲解"什么是正义"
```

### 游戏NPC设计
```
一个性格像张飞的游戏NPC，台词风格要符合他的急性子
```

---

## 安装场景 | Installation

### OpenClaw用户
```bash
# 通过SkillHub安装
skillhub install persona-mimic

# 或手动安装
cp -r characters/ /path/to/openclaw/config/skills/persona-mimic/
cp SKILL.md /path/to/openclaw/config/skills/persona-mimic/
```

### 其他AI平台
JSON文件可独立使用，导入到任何AI对话系统中作为角色预设。

---

## 贡献 | Contributing

欢迎提交PR补充更多人物！

---

## 许可证 | License

MIT License

---

If helpful, please give it a star!
