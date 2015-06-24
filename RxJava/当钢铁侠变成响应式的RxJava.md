当钢铁侠变成响应式的rxjava
============================
系列的这部分内容主要关注于函数式带给我们项目的好处。

像ReactiveX的rxjava框架可以轻松地帮助处理不同的运行环境上运行后台任务或UI线程。在android平台上，这些曾像噩梦一样缠绕我们。

这篇文章同样专注于那些在日常开发中可以尽量缩短你事件的操作符，Reactive Extensions提供非常多的操作符，让你的生活更轻松！

像往常一样，所有的代码和片段都会上传至github，你们可以尽情的评论，提问和吐槽！
[Avengers app on Github](https://github.com/saulmm/Avengers)
在这个系列的第一个部分中，我们聊了聊[Dagger2](http://saulmm.github.io/when-Thor-and-Hulk-meet-dagger2-rxjava-1/)([中文](http://www.devtf.cn/?p=565))。随着我们的深入，我们会发现层之间的耦合会越来越松，而且会提高扩展性。

####RetroLambda

