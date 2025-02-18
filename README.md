AyeRush 是一个用于监控 Warframe 的 EE.log 文件，实时解析赏金任务和月球密室生成情况的工具，并通过图形化界面（GUI）显示任务名称及任务阶段。该工具支持增量刷新，只读取日志中新添加的内容，从而避免重复读取旧日志。

## 功能特点
+ **实时监控日志**  
采用文件监听机制，每次检测到 EE.log 更新后自动读取新增内容。
+ **赏金任务解析**  
从日志中提取任务名称（例如“希图斯 (地球) - 捕获 Grineer 指挥官”）和任务阶段，自动根据任务名称选择对应的阶段映射，生成详细的任务链。
+ **月球密室检测**  
同时解析月球密室相关日志，统计各类密室的生成情况并展示结果。
+ **增量刷新机制**  
支持点击“刷新日志”按钮时，从上次读取位置开始读取新增内容，GUI 上保留已有内容，如果没有新日志则保持当前显示。
+ **图形化界面**  
使用 Tkinter 构建简洁直观的 GUI，方便用户查看任务和密室信息。

