# springboot

### 碎碎念
springboot中的starter可以自己定义，需要写好配置。


## springboot监听机制

Springboot的监听机制，其实是对Java提供的事件监听机制的封装。
Java中的事件监听机制定义了以下几个角色：
- 事件：Event, 继承java.util.EventObject类的对象
- 事件源：Source, 任意对象Object
- 监听器：Listener, 实现对java.util.EventListener接口的对象

Springboot在项目启动时，会对几个监听器进行回调，我们可以实现这些监听器的接口，在项目启动时完成一些操作。

监听器有：
- ApplicationContextInitializer
- SpringApplicationRunListener
- CommandLineRunner
- ApplicationRunner

## springboot监控功能
springboot自带监控功能Actuator，可以帮助实现对程序内部运行状况的监控，比如监控状况、Bean加载情况、配置属性、日志信息。
使用方法，导入actuator坐标

springboot admin提供了一种图形化的界面去分析监控的数据。

actuator和admin在OPs里面添加。