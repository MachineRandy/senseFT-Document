# SenseDaemon 管理后台

{% hint style="info" %}
SenseDaemon 管理后台为管理员权限页面。
{% endhint %}

SenseDaemon 是部署在车辆上的一个 Java 进程服务（实际上是一个 Web 后台服务），该服务主要提供如下几个功能：

1. 通过 Monitor 与 SenseAuto 系统交互
2. 通过 HTTP 与 SenseFT 路测管理系统交互，包括向 SenseFT 转发来自 Monitor 的车辆状态消息
3. 为 SenseDaemon 车载客户端提供后端接口服务

SenseDaemon 管理主要包括两个部分：Tag 标签设置 与 数据采集平台 - 模式设置

Tag 标签是为了结合 SenseDaemon 车载客户端给测试数据打上标记，方便后续数据检索和复用，比如天气，天气又可以分为阴天、雨天和晴天等，根据不同组的需求，有不同的场景。Tag 标签设置这一管理功能是为了能够动态的添加和删除这些 Tag 和 Tag 类别。

数据采集平台 - 模式设置：车辆数据采集与测试任务对应，需要按照不同采集需求（开启不同传感器）和不同的车辆设定不同的采集模式，并将其绑定到每个数据采集类型的任务实例上。这里的模式设置包括生成一个模式，设置这个模式所开启的各类传感器以及对应的车辆。

SenseDaemon 管理后台入口位于[路测管理系统](http://47.103.61.192:80) 导航栏一级菜单项，如图下所示

![SenseDaemon &#x7BA1;&#x7406;&#x540E;&#x53F0;&#x5165;&#x53E3;](.gitbook/assets/image%20%2878%29.png)

Tag 标签设置和数据采集模式设置，操作类似，点击按 **+** 或者 **新增** 按钮，按弹出的提示操作即可。

![Tag &#x6807;&#x7B7E;&#x8BBE;&#x7F6E;&#x4E0E;&#x6570;&#x636E;&#x91C7;&#x96C6;&#x6A21;&#x5F0F;&#x8BBE;&#x7F6E;](.gitbook/assets/image%20%2814%29.png)

![&#x6309;&#x63D0;&#x793A;&#x589E;&#x52A0;&#x548C;&#x5220;&#x9664; Tag &#x548C;&#x6570;&#x636E;&#x91C7;&#x96C6;&#x6A21;&#x5F0F;](.gitbook/assets/image%20%2843%29.png)

