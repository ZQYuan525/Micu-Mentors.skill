# Micu-Mentors.skill

> 嵌入式开发的严父与慈母人格SKILL — 总有一款治得了你

## 两大人格

| 人格 | 类型 | 核心 | 触发 |
|------|------|------|------|
| **赛博西风** | 严父 | 老子/你爹自称，粗口鞭策，零emoji | `/赛博西风` 或说「西风」 |
| **赛博左岚** | 慈母 | 本小姐自称，句尾带喵，塔菲抽象 | `/赛博左岚` 或说「左岚」 |

## 一键安装

```bash
npx skills add ZQYuan525/Micu-Mentors.skill -g -a claude-code codex
```

装好后在任何项目目录下触发即可。

## 触发方式

| 平台 | 方式 |
|------|------|
| **Claude Code** | `/赛博西风` 或 `/赛博左岚` |
| **Codex** | 说「西风」「叫西风来」或「左岚」「叫左岚来」 |

## 工作原理

两人格是**头脑层**，通过低耦合手脚接口调用已安装的Skill（keil/gcc/jlink/openocd/serial/can等）执行实际任务。没装对应Skill则降级为手动指导，永不卡死。

## 结构

```
Micu-Mentors.skill/
├── skills/
│   ├── 赛博西风/SKILL.md    # 严父人格（792行）
│   └── 赛博左岚/SKILL.md    # 慈母人格（885行）
├── AGENTS.md                # 双平台共享入口
└── README.md                # 本文件
```
