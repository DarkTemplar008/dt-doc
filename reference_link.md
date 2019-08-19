#### 图形渲染
* [剖析Unreal Engine超真实人类的渲染技术Part 1 - 概述和皮肤渲染](https://www.cnblogs.com/timlly/p/11098212.html)
* [剖析Unreal Engine超真实人类的渲染技术Part 2 - 眼球渲染](https://www.cnblogs.com/timlly/p/11144950.html)
* [探究光线追踪技术及UE4的实现](https://www.cnblogs.com/timlly/p/11366199.html)
> 光栅化技术是使用主观方法对三维世界的描述，而光线追踪算法是使用比较客观的方法对三维世界的描述，逻辑简单但计算复杂


#### Chromium
* [Life of a Pixel 2018](https://docs.google.com/presentation/d/1boPxbgNrTU0ddsc144rcXayGA_WF53k96imRH8Mp34Y/edit#slide=id.p)
  > h5是如何从代码变成图片的
* [Smart Pointer Guidelines](https://www.chromium.org/developers/smart-pointer-guidelines)
  > chromium并不推荐在多线程环境下使用引用计数技术，因为chromium的设计理念是线程拥有资源，资源的生命周期约束在线程的生命周期里面，线程间传递消息通过值拷贝方式来实现


#### 编译器技术
* [include-what-you-use](https://include-what-you-use.org/)
  >优化头文件的辅助工具
* [distcc](https://github.com/distcc/distcc)
  >gcc分布式编译器
* [为什么多线程读写 shared_ptr 要加锁？](http://www.cppblog.com/Solstice/archive/2013/01/28/197597.html)
  >对shared_ptr线程安全性做了论述，shared_ptr本身是线程安全的，解引用后肯定线程不安全，deleter也不一定线程安全，作为生产者消费者模型还是不错的
  
#### Qt
* [Qt_5_on_Windows_ANGLE_and_OpenGL](https://wiki.qt.io/Qt_5_on_Windows_ANGLE_and_OpenGL)
  > Qml默认使用OpenGL作为渲染引擎，OpenGL在Windows平台上总是掉链子，需要使用ANGLE来做转换，ANGLE是Chrome底层OpenGL封装库，在Windows上ANGLE将OpenGL转换为DirectX调用
* [Dynamic OpenGL implementation loading in Qt 5.4](https://blog.qt.io/blog/2014/11/27/qt-weekly-21-dynamic-opengl-implementation-loading-in-qt-5-4/)
  > 动态加载OpenGL或者ANGLE
  
  
#### OllyDbg
* [OllyDbg-基础](https://www.hirworld.xyz/posts/aea6ff50/)
  > OllyDbg基本介绍
  
#### Windows
* [api-ms-win-core files](https://www.nirsoft.net/articles/windows_7_kernel_architecture_changes.html)
  > api-ms-win-core*.dll文件列表详细描述，应该是安全方面的考虑，具体原因待更新
* [Dependencies](https://github.com/lucasg/Dependencies)
  > Win10系统上的Depends实在是太慢了，有牛人重新开发了一个新的Depends，实测速度非常快，解压后运行DependenciesGui.exe
  
#### go
* [GoForCPPProgrammers](https://github.com/golang/go/wiki/GoForCPPProgrammers)
  > Go跟C++进行类比，对于C++开发者来说这样的类比是非常适合入门Go的，比直接看Go的神奇的语法有意思得多，也深刻得多，Go确实在服务端开发方面比C++来的简洁，一个channel功能就能释放C++多少代码
