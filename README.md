



# [简体中文](https://github.com/Anteayer/spanish-vocab-wallpaper)                                [Español](https://github.com/Anteayer/spanish-vocab-wallpaper/tree/master/docs)



# spanish-vocab-wallpaper



#### 所有信息来源:  http://www.esdict.cn/



#### 项目大概架构: Python 3.7 + Cefpython3 + Web



#### 使用方法:

1. 使用项目中 existence/run/run.exe 便会运行程序



#### 注意事项:

1. 需要关闭程序时，从任务管理器结束 run.exe 或者自己编写 bat 文件来结束
2. Cefpython3 目前最高只支持 Python 3.7
3. 执行程序时会初始化一张壁纸，之后便会显示单词
4. 请勿在短时间内多次执行程序，短时间调用多次将会导致单词信息中出现各种不明的文字图片影响观看 (网站反爬机制)
5. 壁纸可以自由更改，但是单词卡片也许会不适配你自己选用的壁纸，可以自己设计 web UI



#### 写这个项目的坑：

1. 首先是处理将 cef 浏览器窗口绘制到桌面时，为了实现触发网页 hover 的时候，在发送鼠标消息时 (PostMessage)， Windows 会自动产生一个鼠标离开的事件，导致排查了许久
2. python 的一个坑，初始化类数组时，有一种写法，python 会在同一内存地址中初始化所有的类数组，结果导致了有时候类数组中的某一对象为 None 时，会莫名引用同一内存地址中其他对象的数值




![yscJpV.gif](docs/exp.gif)
