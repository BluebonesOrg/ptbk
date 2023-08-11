# 介绍
这是一个 Matlab 包，它对 PsychToolbox 的部分api进行组合封装，可以提高 PsychToolbox 程序开发速度并降低bug率

详细使用方法见 [API文档](./ "还没写")

# 安装
请先确保 Matlab 安装了 PsychToolbox 

**方法1** 把`+PTB`文件夹和实验程序在同一文件夹下

**方法2** 把`+PTB`文件夹路径添加到matlab搜索路径中

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
