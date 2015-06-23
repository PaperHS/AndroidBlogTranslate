
## 为什么我们要避免使用eventbus


原文：[endlesswhileloop](http://endlesswhileloop.com/blog/2015/06/11/stop-using-event-buses/) 
翻译：[Paper](https://github.com/PaperHS)

我在android开发中最常见到的一种模式就是eventbus。一些库（像otto，eventbus）常常被使用以便可以移除一些穿越多层的回调函数。虽然它们一开始的时候都非常管用，但是很快，他们就会被陷入庞大且复杂的事件管理的麻烦中，而且还难以追踪和调试。
eventbus经常被宣传为可以帮助你实现松耦合设计，但是实际上它带给你的是松耦合的混乱和紧耦合的缺点。

#### 嵌套事件
一个常见的陷阱就是嵌套事件。这看上去似乎很好避免，只要不在subscriber中发送事件，但是这个问题通常没有这么好解决。一个订阅可能调用了一个方法，而这个方法又间接的发送了一个事件。这些杂乱的事件令人难以置信的的复杂和难以调试。
Facebook的Flux架构也是事件驱动，但是它明确的禁止发送嵌套事件。我希望otto和eventbus也能这么做。

#### 把生产者当做同步获得者
（我不认为这和GreenRobot的eventbus相关）
这是另外一种不可能在大项目中不出现的常见模式。


  
