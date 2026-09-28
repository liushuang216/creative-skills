# Creative Skills

可复用的创意类 Agent Skills，面向支持 `SKILL.md` 的助手。

## 当前技能

| Skill | 用途 |
| --- | --- |
| [photo-doodle-poster](skills/photo-doodle-poster/SKILL.md) | 每张照片生成一张 3:4 海报：上半照片，下半少色极简手绘；上下等分，主体完整，大量留白。 |

## 安装到 Codex

将本仓库下载或克隆后，将需要的 skill 文件夹复制到个人 skills 目录：

```bash
git clone https://github.com/liushuang216/creative-skills.git
mkdir -p ~/.codex/skills
cp -R creative-skills/skills/photo-doodle-poster ~/.codex/skills/
```

已有同名 skill 时，先比较内容，再决定是否替换。重新启动会话后调用：

```text
使用 $photo-doodle-poster，把这些照片分别做成独立海报。
```

也可仅生成 prompt：

```text
使用 $photo-doodle-poster，为这张照片写一份无字版本的生成提示词。
```

需要生成图片时，运行环境须提供支持参考照片的图像编辑工具。只有文字能力的环境可以使用提示词模板。

## 设计原则

保留原始审美 prompt，并纳入实际迭代中的主体完整性修正。删减背景和细节，不误删主要主体的腿脚；靠缩小主体与扩展环境适配画幅。尺寸和分区仍需检查生成结果，文字约束不保证每次生成都精确满足。

仓库仅包含通用技能与文本模板，不附带私人照片或人像成品。

## License

MIT

