# 介绍

这是一个 Matlab 包，它对 PsychToolbox 的部分 api 进行组合封装，可以提高 PsychToolbox 程序开发速度并降低 bug 率

详细使用方法见 [API 文档](./ '还没写')

# 安装

请先确保 Matlab 安装了 PsychToolbox

**方法 1** 把`+PTB`文件夹和实验程序在同一文件夹下

**方法 2** 把`+PTB`文件夹路径添加到 matlab 搜索路径中

# 示例代码

```matlab
app = PTB.App(); % 构建app
app.debug(); % 启动debug模式
app.backgroundColor = [255 255 255]; % 背景色设为白色
app.begin(); % 启动app
app.Element.multiText('欢迎参加实验\n请按空格键开始'); % 绘制多行文本
app.Element.render(inf); % 渲染绘制内容，并启动键盘监听
app.finish(); % 结束app
```

# 需求分析

呈现刺激

-   刺激类型
-   呈现时机
-   呈现控制
-   监听输入
-   消失时机
