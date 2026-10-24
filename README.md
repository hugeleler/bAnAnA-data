# bAnAnA-data

方案数据。软件版本在 bAnAnA-mac、bAnAnA-windows、bAnAnA-android，不在这个库发布。

```
banana/themes/*.bskin
frost/themes/*.bskin
```

每个方案 12 个 bskin，直接放在 `themes/` 下，不再按 mac、windows 分子目录。一个 bskin 是一份 zip，里面按环境分块：`android`、`ios`、`mac`、`windows`。没有哪一块，那个环境就不加载这份文件。十个桌面皮肤四块都有。`rainbow.bskin` 和 `banana.bskin` 只有 android 和 ios。

下载地址是 `https://raw.githubusercontent.com/hugeleler/bAnAnA-data/main/{方案}/themes/{id}.bskin`。`catalog.json` 里每条 theme 仍带 `platform`，客户端只取自己这个环境的条目。`version` 和文件里的 `manifest.yaml` 一致。换皮肤时改这个版本并替换文件，不要改小香蕉的软件版本号。

语言模型不在 git 目录里。git 单文件上限 100MB，`banana-lts-zh-hans.gram` 是 398MB。两个 gram 挂在本库 Release `language-model` 的附件上。

以后加方案：新建顶层目录，例如 `moqi/`，再往 `catalog.json` 增加该方案的 gram 和 theme 条目。
