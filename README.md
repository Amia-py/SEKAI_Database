# SEKAI Datebase

PJSK（プロジェクトセカイ カラフルステージ！ feat. 初音ミク / HATSUNE MIKU: COLORFUL STAGE! / 初音未来：缤纷舞台）全资料库。
**中・日・英三语** × **TXT / JSON / Markdown / SQLite** 四格式，每个最小单元同时提供四种载体。

PJSK full database, **trilingual (zh / ja / en)** × **TXT / JSON / Markdown / SQLite**, every minimal unit provided in all four formats.

プロジェクトセカイの総合データベース。**中・日・英3言語** × **TXT / JSON / Markdown / SQLite** の4形式で、最小単位ごとに4種のファイルを同梱。

---

## 目录结构 / Structure / ディレクトリ構成

```
SEKAI_Datebase/
├─ 中文/            中文数据（文件名与内容均为中文，取自国服官方文本）
│  ├─ 简介/         游戏简介、世界观、各服上线信息
│  ├─ 剧情/
│  │  ├─ 主线/      主线剧情（按组合 → 章节 → 话）
│  │  ├─ 活动/      活动剧情（箱活 / 混活 / WL）
│  │  └─ 卡牌/      卡牌剧情（按角色聚合）
│  ├─ 角色/         每个角色：基本设定 / 剧情 / 卡面 / 红线
│  ├─ 卡面/         按角色 → 旧队服·新队服·1/2/3/4星·生日·特典·联动 分类
│  ├─ 音乐/         原创（含「箱曲」子分类） / 翻唱
│  ├─ MV_PV/        MV 出演角色与资源索引
│  ├─ 开发商解释/    SEGA / Crypton Future Media / Colorful Palette / 朝夕光年
│  └─ 特殊事件/      国服（朝夕光年）运营事件记录
├─ 日文/            日本語データ（同上结构，取自日服官方文本）
├─ 英文/            English data (same structure, from the EN server text)
├─ 日文/カード/画像/  卡面图片（仅一份，三语通过相对路径引用）
└─ SEKAI_Datebase.db  汇总数据库
```

**最小单元**示例（角色基本设定）：

```
中文/角色/瑞希/基本设定/
├─ 瑞希_基本设定.txt
├─ 瑞希_基本设定.json
├─ 瑞希_基本设定.md
└─ 瑞希_基本设定.db
```

## 数据说明 / Data Notes / データについて

| 项目 | 中文 | 日文 | 英文 |
|---|---|---|---|
| 数据来源 | 国服 master（pjsk.nvsgames.cn） | 日服 master（pjsekai.sega.jp） | 国际服 master（colorfulstage.com） |
| 进度 | 落后日服，部分内容标注缺失 | 最全 | 落后日服约一年 |

- 各服进度不同：以日服 ID 为基准对齐，国服／国际服尚未实装的条目会在对应语言包中缺失。
- 剧情正文仅提取 **说话人、说话内容、背景变化、内心独白** 四类要素，保留官方原文，不作改写。
- 图片为小尺寸 webp（约 67/103KB），存放于 `日文/カード/画像/`，三语共用。
- 音频／曲绘等大体积媒体以官方资源 URL 形式索引（仓库内不重复存放大文件）。

## 数据来源 / Sources / 出典

- 国服官网 https://pjsk.nvsgames.cn/
- 日服官网 https://pjsekai.sega.jp/
- 国际服官网 https://www.colorfulstage.com/
- SEKAI Viewer https://sekai.best/
- Moesekai https://pjsk.moe/
- SEKAI master database（Sekai-World/sekai-master-db-diff、sekai-master-db-cn-diff、sekai-master-db-en-diff）
- SEGA 官方新闻稿、Crypton / Colorful Palette / 朝夕光年 官网
- 国服运营事件：什么值得买社区、TapTap 社区、NGA 玩家社区等公开报道（客观转述）

## 免责声明 / Disclaimer / 免責事項

本项目仅作资料整理与检索用途，所有文本、图片、音频的著作权归 SEGA、Colorful Palette、Crypton Future Media 及各权利方所有。

This project is for reference and archival purposes only. All text, images, and audio are the property of SEGA, Colorful Palette Inc., Crypton Future Media, INC. and their respective rights holders.

本プロジェクトは資料整理・検索目的のみです。すべてのテキスト・画像・音声の著作権は SEGA、Colorful Palette、クリプトン・フューチャー・メディアおよび各権利者に帰属します。
