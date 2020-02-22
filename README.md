## 智能播放器
通过手势的变化操控播放器的不同功能。此版本不是最后的，仍然需要更新

## 需要准备的材料
1.播放器代码 \n
2.手势模块驱动  \n
3.mplayer移植文件 \n
4.相关素材  \n
5.PAJ762U2手势识别传感器 \n

## 使用说明
1.将mplayer移植到开发板 (放至/bin/目录 并赋予权限 chmod 777 mplayer)
2.将素材放到开发板 （我已经指定好路径，请将主界面的素材放至根目录的/myphoto/, 音乐界面的素材放至根目录的/mymusic/, 视频界面的放至根目录的/myvideo/）
3.将手势模块驱动下载至开发板，或编译进内核  insmod IIC_drv.ko 安装驱动
4.将播放器代码中的play_work下载到开发板，并赋予权限 chmod 777 ./play_work
5.用杜邦线将手势传感器与开发板连接

这样就可以使用了
注意事项：不要使用QT编译播放器代码，要使用QT交叉编译来编译。

## 手势说明
向左向右是选择不同的按键
向上是点击按键，选中音视频列表时，是选择不同音视频
向下是退出界面，选中音视频列表时，是选择不同音视频
向前是播放音视频 
晃动是视频的全屏模式
注意：全屏模式时，向下是退出全屏，且只能响应向下的手势
