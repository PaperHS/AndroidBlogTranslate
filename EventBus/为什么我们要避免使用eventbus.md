
## 为什么我们要避免使用eventbus


原文：[endlesswhileloop](http://endlesswhileloop.com/blog/2015/06/11/stop-using-event-buses/) 
翻译：[Paper](https://github.com/PaperHS)

我在android开发中最常见到的一种模式就是eventbus。一些库（像otto，eventbus）常常被使用以便可以移除一些穿越多层的回调函数。虽然它们一开始的时候都非常管用，但是很快，他们就会被陷入庞大且复杂的事件管理的麻烦中，而且还难以追踪和调试。

  
