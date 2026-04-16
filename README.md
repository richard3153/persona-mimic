# persona-mimic / 人格预设库

> AI角色扮演数据库 — 1000位世界名人的思维模式与说话风格

## 内容

- **1000位名人** 来自8个领域
- 每个人物包含: `name`, `zhName`, `years`, `field`, `core`(核心特质), `thinking`(思维方式), `speaking`(说话风格), `solving`(解决问题方式), `quotes`(经典语录), `recommended_skills`(推荐技能标签)

## 目录结构

```
characters/
├── 01_scientists.json    科学家与发明家 (160人)
├── 02_artists.json       艺术家与音乐家 (55人)
├── 03_entrepreneurs.json 企业家与商业领袖 (133人)
├── 04_athletes.json      运动员 (246人)
├── 05_writers.json       作家与思想家 (90人)
├── 06_actors.json        演员与导演 (124人)
├── 07_historical.json    历史人物 (66人)
└── 08_others.json        其他领域名人 (126人)
```

## 技能标签

- `athlete_basketball` 篮球
- `musician_pop` 流行音乐
- `actor_classical` 演员
- `entrepreneur_tech` 科技企业家
- `scientist_ai` AI/计算机
- `writer` 作家
- `director` 导演
- `philosopher_western` 西方哲学家
- `philosopher_chinese` 中国哲学家
- `politician_democratic` 政治家
- `military_commander` 军事家
- `activist` 社会活动家
- 等等...

## 使用方法

在OpenClaw中，通过`persona-mimic`技能使用这些预设。

## License

MIT
