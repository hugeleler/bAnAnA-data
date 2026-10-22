# bAnAnA-data

方案数据。软件版本在 bAnAnA-mac、bAnAnA-windows，不在这个库发布。

```
banana/themes/mac/*.bskin
banana/themes/windows/*.bskin
frost/themes/mac/*.bskin
frost/themes/windows/*.bskin
```

Mac 和 Windows 的皮肤文件名相同，所以按平台分子目录。

语言模型不在 git 目录里。git 单文件上限 100MB，`banana-lts-zh-hans.gram` 是 398MB。两个 gram 挂在本库 Release `content` 的附件上。

方案版本是 `catalog.json` 里的 `version`。换皮肤或换 gram 时改这个版本并替换文件，不要改小香蕉的软件版本号。

以后加方案：新建顶层目录，例如 `moqi/`，再往 `catalog.json` 增加该方案的 gram 和 theme 条目。
