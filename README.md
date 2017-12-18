
EasyGUI是Python的一个简单易用的图形模块。和其它的GUI不同，EasyGUI没有事件驱动。而且，所有的GUI交互都是通过简单的函数来调用的。

EasyGUI可以在Python 2和Python 3上运行，无其它任何依赖。

终端用法示例：

===============

 #-*-coding:UTF-8-*-

 >>> import easygui

 >>> easygui.ynbox('继续?', '标题', ('是', '否'))

 True

 >>> easygui.msgbox('此为简单的message box.', '标题在此')

 'OK'

 >>> easygui.buttonbox('选择你最爱的歌手','最爱歌手', ('洛天依', '乐正绫', '星尘'))

 '星尘'

===============
