Engines
=======

binge使用Rails Engine将应用分为几个部分：

core <- backend
core <- frontend <- web

core是应用的核心，包含Model数据，还有会被前后台同时用到的逻辑。

backend是一个Rails App，包含后台管理用的Controller逻辑。

类似地，frontend存储前台逻辑，主要以Service形式存储。

web和未来可能会有的api则调用frontend里的service来完成业务，这两项应该只包含controller和view逻辑。