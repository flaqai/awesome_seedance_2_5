# Seedance 2.5 多语言 Prompts 目录

[返回 60 场景索引](../README.md) · [返回主指南](../../README.md) · [在线使用](https://flaq.ai/models/bytedance/seedance-2-5-image-to-video/)

这里的每个语言文件均包含 6 个完整提示词，覆盖产品广告、时尚、电商 UI、科普、房地产和宠物场景。它们保留相同的场景 ID 与制作约束，方便团队逐语言测试提示词理解、对白、音频和本地化表现。

## 语言文件

| 语言 | 文件 | 方向 |
|---|---|---|
| 繁體中文 | [prompt-library.zh-TW.md](prompt-library.zh-TW.md) | LTR |
| English | [prompt-library.en.md](prompt-library.en.md) | LTR |
| 日本語 | [prompt-library.ja.md](prompt-library.ja.md) | LTR |
| 한국어 | [prompt-library.ko.md](prompt-library.ko.md) | LTR |
| Español | [prompt-library.es.md](prompt-library.es.md) | LTR |
| Français | [prompt-library.fr.md](prompt-library.fr.md) | LTR |
| Deutsch | [prompt-library.de.md](prompt-library.de.md) | LTR |
| Português do Brasil | [prompt-library.pt-BR.md](prompt-library.pt-BR.md) | LTR |
| العربية | [prompt-library.ar.md](prompt-library.ar.md) | RTL |
| Русский | [prompt-library.ru.md](prompt-library.ru.md) | LTR |
| Bahasa Indonesia | [prompt-library.id.md](prompt-library.id.md) | LTR |

## 六个共享场景

| ID | 场景 | 重点 |
|---|---|---|
| I18N-01 | 无品牌气泡茶广告 | 产品几何、玻璃、液体、声音同步 |
| I18N-02 | 防雨风衣风场测试 | 身份、服装、风向与布料物理 |
| I18N-03 | 专注计时器 UI 演示 | 文字保真、状态转换、光标操作 |
| I18N-04 | 城市湿地科普 | 科学准确、箭头、标签与免责声明 |
| I18N-05 | 小户型真实导览 | 平面图、空间尺度、诚实镜头 |
| I18N-06 | 老年犬雨衣检查 | 宠物身份、温和操作、产品合身 |

## 本地化规则

1. `Image 1`、`Video 1`、`Audio 1` 等素材编号保持固定，必须与上传顺序一致。
2. 镜头方向、动作、音频、一致性和禁止项要一起翻译，不能只翻译风格词。
3. 需要出现在画面中的文字必须放在引号中，并注明目标语言；不需要文字时明确写“无字幕、无伪文字”。
4. 产品几何、界面字段、型号、文件名和已批准的品牌拼写不应自由改写。
5. 阿拉伯语等 RTL 内容要单独定义阅读方向；镜头左右方向不要因为文字方向自动镜像。
6. 涉及服装、手势、食物、建筑、地理、无障碍、健康或公共安全时，应由熟悉当地语境的人复核。

## 人工检查

- 每个语言版本是否保留了相同的素材职责；
- 对白是否自然，口型与语速是否适合目标语言；
- UI、标点、数字和单位是否准确；
- 是否意外删除了版权、安全或一致性限制；
- 是否生成了不必要的字幕、商标、价格或事实声明；
- RTL 版本的 UI 阅读方向与镜头空间方向是否分别处理。
