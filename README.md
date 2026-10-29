> 📦 **已归档（Archived — 仅作参考）**
> 本仓库已收入归档仓 **media-prototypes**（代码与完整 git 历史一并迁入，原仓冻结不再开发）。
> 历史分支见归档仓的 `archive/photovideo` 分支；活跃维护请前往 **media-prototypes**。
> _This repo is archived into media-prototypes; development continues there. Do not commit here._

# photovideo

> 仓库：<https://gitee.com/siwpan/photovideo> ｜ 许可：MIT（见 [LICENSE](LICENSE)）

图片转视频生成器 —— 把多张图片合成视频的 Tkinter 工具，内置 6 种动效模式（网格拼贴、横/纵长图滚动、淡入淡出、KenBurns 推镜、逐张高亮）。

## 语言 / 类型
- Python（Tkinter GUI + ffmpeg 命令行合成）

## 目录要点
- `main.py` —— 入口（`App().mainloop()`）；`app.py` —— 主 GUI（6 种模式）
- `core.py` —— 图片加载/时长等基础函数；`compositors.py` —— 网格拼贴/长图/高亮素材生成
- `ffmpeg_utils.py` —— ffmpeg 进度调用封装；`1.py` —— 早期脚本
- `output/`、`outputs/` —— 输出目录

## 运行方式与依赖
- 运行：`python main.py`
- 依赖：`Pillow`、tkinter 标准库，以及系统 `ffmpeg`（需在 PATH 中，程序会自行探测）。无 requirements.txt。

## 测试状态
- `py_compile` 语法检查通过（6 个 .py 文件）。
- GUI 程序（依赖 ffmpeg），本次仅编译未运行。
