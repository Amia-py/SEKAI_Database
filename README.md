# SEKAI Datebase

PJSK（プロジェクトセカイ カラフルステージ！ feat. 初音ミク / HATSUNE MIKU: COLORFUL STAGE! / 初音未来：缤纷舞台）全资料库。
**中文・English・日本語** 三大分类 × **TXT / JSON / Markdown / SQLite** 四格式，每个最小单元同时提供四种载体，图片与音频等资源以实际文件形式存放于各语言目录内。

PJSK full database, organized as **中文 / English / 日本語** × **TXT / JSON / Markdown / SQLite**, every minimal unit in all four formats, with images and audio stored as real files inside each language folder.

プロセカ総合データベース。**中文 / English / 日本語** × **TXT / JSON / Markdown / SQLite** の4形式で、画像・音源は各言語フォルダ内に実ファイルとして同梱。

---

## 目录结构 / Structure / 構成

```
SEKAI_Datebase/
├─ 中文/              中文数据（取自国服官方文本）
│  ├─ 简介/           游戏简介、世界观、各服上线信息
│  ├─ 剧情/
│  │  ├─ 主线/        主线剧情（组合 → 章节 → 话）
│  │  ├─ 活动/        活动剧情（箱活 / 混活 / WL）
│  │  └─ 卡牌/        卡牌剧情（按角色聚合）
│  ├─ 角色/           每个角色：基本设定 / 剧情 / 卡面 / 红线
│  ├─ 卡面/           按角色 → 旧队服·新队服·1/2/3/4星·生日·特典·联动 分类
│  │  └─ {角色}/图片/  卡面图片（实际文件）
│  ├─ 音乐/           原创（含「箱曲」） / 翻唱
│  │  └─ 音频/        试听音频（实际文件）
│  ├─ MV_PV/          MV 出演角色与资源索引
│  ├─ 开发商解释/      SEGA / Crypton Future Media / Colorful Palette / 朝夕光年
│  └─ 特殊事件/        国服（朝夕光年）运营事件记录
├─ English/           English data (from the EN server, same structure)
├─ 日本語/            日本語データ（日本サーバー公式テキスト、同構造）
└─ README.md
```

**最小单元**示例（角色基本设定）：

```
中文/角色/瑞希/基本设定/
├─ 瑞希_基本设定.txt
├─ 瑞希_基本设定.json
├─ 瑞希_基本设定.md
└─ 瑞希_基本设定.db
```

## 资源说明 / Resources / リソース

- **卡面图片**：小尺寸 webp（特训前约 67KB / 特训后约 103KB），存于各语言目录 `卡面/{角色}/图片/`（日本語：`カード/{キャラ}/画像/`，English: `Cards/{char}/Images/`），文件名格式 `{卡面ID}_{卡名}_{normal|trained}.webp`，三语各自完整一份。
- **试听音频**：short 版 mp3（每首约 0.5MB），存于各语言目录 `音乐/音频/`（日本語：`楽曲/音源/`，English: `Music/Audio/`），文件名 `{曲ID}_{曲名}.mp3`，按各语言曲名命名。
- **完整版音频 / MV 视频**：体积过大，以官方资源 URL 形式在索引中提供（storage.sekai.best）。
- 剧情正文仅提取 **说话人、说话内容、背景变化、内心独白** 四类要素，保留官方原文，不作改写。

## 数据进度 / Server Progress / サーバー進行

| 项目 | 中文 | 日本語 | English |
|---|---|---|---|
| 数据来源 | 国服 master（pjsk.nvsgames.cn） | 日服 master（pjsekai.sega.jp） | 国际服 master（colorfulstage.com） |
| 进度 | 落后日服，未实装内容缺失 | 最全 | 落后日服约一年 |

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
