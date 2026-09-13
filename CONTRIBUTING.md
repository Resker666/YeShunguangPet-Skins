# 投稿与收录

## 创作者投稿

1. 在主程序里预览待机、点击、拖动和其他已配置动作。
2. 使用「导出皮肤 ZIP」，不要打包整个应用目录或个人设置目录。
3. 打开 [皮肤投稿表单](https://github.com/Resker666/YeShunguangPet-Skins/issues/new?template=submit-skin.yml)，提交预览和 ZIP。
4. 如需修正，在原投稿中补充新版本，保持角色 ID 不变。

推荐 ID 使用 `作者-角色`，例如 `resker666-hutao`，避免不同创作者使用同一个 ID。已经发布或使用中的 ID 不应随意更改。显示名称可以使用中文。

## 皮肤包约定

```text
resker666-hutao/
  pet.json
  spritesheet.png
```

ZIP 内只能有一个 `pet.json`，PNG 必须与它同目录，实际文件名由 `spriteSheet` 字段指定。可以使用上述单层角色目录，也可以直接放在 ZIP 根目录。

当前主程序限制：ZIP 压缩大小及全部解压条目总大小分别不超过 80 MiB，最多 256 个条目。其余尺寸与字段限制以 [主程序皮肤格式](https://github.com/Resker666/YeShunguangPet/blob/main/docs/PET_FORMAT.md) 为准。

版本、作者和许可写在本仓库的角色说明页中。不要直接向 `pet.json` 添加不受支持的字段；主程序会拒绝未知字段。

## 维护者收录

1. 核对作者署名、来源和分发说明；存在不明确之处先与投稿者沟通。
2. 使用主程序自带的 `scripts/validate-skin.ps1` 校验 ZIP，再实际导入预览。
3. 从 [说明模板](templates/SKIN_README.md) 新建 `skins/<id>/README.md`，加入预览、原始清单和 PNG，并参照胡桃条目添加 `release.json`。
4. 提交并推送源文件后，再推送皮肤标签，例如 `resker666-hutao-v1.0.0`。标签 ID、清单 ID、`release.json` 的 ID 和版本必须匹配。
5. 等待 Release skin 自动流程校验并生成 ZIP 和 SHA256 文件，确认发布成功，再将真实下载链接填回角色说明和首页目录。
6. 在投稿中告知收录结果；后续更新使用新版本标签和附件，不静默替换旧版本。

## 分享范围

皮肤投稿只包含角色资源，不包含 API Key、AI 聊天记录、个人桌面配置、日志、可执行程序或安装脚本。主程序的皮肤导出功能只导出清单和 PNG；分享前仍请核对 ZIP 内容。
