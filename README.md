# Video QC System (视频质量自动检测系统)

项目简介
基于Flask和OpenCV开发的本地化视频质量检测工具。
主要用于批量扫描文件夹，自动验证视频文件是否符合实验室的数据采集标准：分辨率、帧率、时长、命名规范等。

核心功能：
1.格式检查：验证 MP4/MOV/AVI/MKV 格式。
2.参数核验：标准设定为 4K (4:3比例), 30FPS。
3.时长统计：自动计算有效采集时长，判定是否满足“单文件夹≥6小时”和“平均≥7小时”的标准。
4.跨平台兼容：适配 Windows (Tkinter弹窗) 和 macOS (AppleScript弹窗)。

环境依赖与安装
项目使用 Python 3.8+ 版本。
根目录下有 `requirements.txt` 文件，可运行以下命令安装所需库：
pip install -r requirements.txt
