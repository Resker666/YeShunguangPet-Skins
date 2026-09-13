# 桌面宠物 · 社区皮肤库

为 [YeShunguangPet](https://github.com/Resker666/YeShunguangPet) 桌面宠物分享角色皮肤、动画和创作经验。

[下载主程序](https://github.com/Resker666/YeShunguangPet/releases/latest) · [下载皮肤](https://github.com/Resker666/YeShunguangPet-Skins/releases) · [投稿皮肤](https://github.com/Resker666/YeShunguangPet-Skins/issues/new?template=submit-skin.yml) · [制作与格式说明](https://github.com/Resker666/YeShunguangPet/blob/main/docs/PET_FORMAT.md)

## 皮肤目录

| 角色 | 作者 | 版本 | 下载与介绍 |
| --- | --- | --- | --- |
| 胡桃 | Resker666 | 1.4.0 | [查看皮肤](skins/hutao/README.md) |

社区皮肤按需下载，不会自动加入主程序的内置角色，也不会要求用户重新编译程序。

## 下载与使用

1. 从本仓库 Releases 下载想要的**单角色 ZIP**，不要下载 GitHub 自动生成的 Source code。
2. 打开桌宠控制中心，在皮肤管理中选择「导入皮肤」，选中下载的 ZIP。
3. 预览动作后添加到桌面。更新同一角色时使用「更新皮肤」。

没有单独的安装程序；皮肤包只需要 `pet.json` 和清单引用的 PNG。

## 分享你的角色

先在主程序中使用「导出皮肤 ZIP」，再通过上方「投稿皮肤」提交：

- 角色名称、唯一 ID、版本和作者署名。
- 一张预览图或演示 GIF，以及皮肤 ZIP 的下载链接或附件。
- 素材来源、使用范围、是否允许收录分发、是否允许修改。
- 建议使用的主程序版本和已知问题。

维护者校验格式并预览后收录。投稿不自动等于收录。具体步骤见 [投稿说明](CONTRIBUTING.md)。

## 仓库如何组织

```text
skins/
  作者-角色/
    README.md       # 预览、作者、版本、来源与下载链接
    preview.png     # 轻量预览图（也可用 GIF 或完整精灵图）
    pet.json        # 收录后的皮肤清单
    spritesheet.png # 与清单配套的 PNG
    release.json    # 独立版本、署名与校验版本
Releases            # 单角色 ZIP 下载包
```

Git 仓库保存目录、说明和皮肤源文件，完整皮肤 ZIP 放在 Releases。每个皮肤可以独立更新，不跟随主程序版本号。推送 `<皮肤ID>-v<版本>` 标签后，自动流程会校验并打包清单和 PNG，发布 ZIP 与 SHA256 校验文件。

本阶段通过网页浏览、下载并在程序中导入；应用内在线皮肤商店尚未实现。

## 素材说明

每份皮肤的素材来源和使用范围以该皮肤页面为准，详见 [素材说明](ASSET_POLICY.md)。本仓库不对所有角色图片统一授予 MIT 或其他素材许可。
