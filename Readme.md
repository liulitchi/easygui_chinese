
EasyGUI是Python的一个简单易用的图形模块。和其它的GUI不同，EasyGUI没有事件驱动。而且，所有的GUI交互都是通过调用简单的函数完成的。

EasyGUI可以在Python 2和Python 3上运行，无其它任何依赖。

## 终端用法示例：

```
#-*- coding:UTF-8 -*-
>>> import easygui
>>> easygui.ynbox('继续?', '标题', ('是', '否'))
True
>>> easygui.msgbox('此为简单的message box.', '标题在此')
'OK'
>>> easygui.buttonbox('选择你最爱的歌手','最爱歌手', ('洛天依', '乐正绫', '星尘'))
'星尘'
```

## 如何安装：

最直接的方式(Python2): > pip install --upgrade easygui

在Python3下：> pip3 install --upgrade easygui

即可获取最新版的easygui。

也可以去sourceforge下载:

`https://sourceforge.net/projects/easygui/files/`


## easygui API

### 按钮框 (buttonbox):

```
easygui.buttonbox(msg='', title=' ', choices=('Button[1]', 'Button[2]', 'Button[3]'), 
                  image=None, images=None, default_choice=None, 
                  cancel_choice=None, callback=None, run=True)
  
  Display a msg, a title, an image, and a set of buttons. 
  The buttons are defined by the members of the choices global_state.
  ```
  
 ###  可选参数：
  
- msg (str) :显示的信息
-  title (str) : 窗口标题
- choices (list) : 可选的一列元组
-  image (str) : 图像文件名，为了兼容旧版
-  images (str) : 图像文件名,可以迭代选择
- default_choice (str) : 默认选项
- 返回值: 用户点击的选项

### 对话框 (dialog openbox)： 

> easygui.diropenbox(msg=None, title=None, default=None)

### 可选参数： 

- msg (str) : 显示的消息
- title (str) : 窗口标题
- default (str) :打开对话框的起始目录
- 返回值: 用户选择的文件路径

### file openbox：

```
easygui.fileopenbox（msg = None，title = None，default ='*'，
                    filetypes = None，multiple = False ）
  ```

