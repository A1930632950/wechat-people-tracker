# data 目录说明

本目录存放所有人物档案数据（隐私数据，仅在本地使用，不外传）。

```
data/
├── index.md       人物总索引
├── people/        每人一个档案 PXXXX-姓名.md（模板见 ../templates/person-profile.md）
├── sources/       每次上传的原始聊天文本 BXXXX.md（溯源用）
├── followups.md   待跟进清单（B版提醒单）
└── backup/        每次更新前的自动备份 BXXXX-<YYYYMMDD-HHMM>/（先备份后写入，可回滚）
```

- 人物 ID（PXXXX）与批次 ID（BXXXX）、事件 ID（EXXXX）均只增不复用。
- `index.md`、`followups.md` 首次使用时从 `../templates/` 复制同名文件初始化。
- 本目录除 `.gitkeep` 与说明外全部被 `.gitignore` 排除：真实聊天记录与他人隐私只存本地，不进入公开仓库。
