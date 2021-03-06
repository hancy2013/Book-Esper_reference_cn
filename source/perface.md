**目录** 
========
* 1.技术概览
 - 1.1 [CEP介绍 & 解析事件流]()
 - 1.2 [CEP与数据库]()
 - 1.3 [Esper引擎]()
 - 1.4 [第三方依赖库]()
* 2.事件展现形式
 - 2.1 [用Java对象表示事件]()
 - 2.2 [事件属性]()
 - 2.3 [事件的动态属性]()
 - 2.4 [Fragment 和 Fragment类型 (是否翻译为碎片?)]()
 - 2.5 [POJO 对象事件]()
 - 2.6 [java.util.Map 事件]()
  - 2.6.1 [概要](2.6.1.md)
  - 2.6.2 [map事件的事件属性](2.6.2.md)
  - 2.6.3 [map事件中的高级属性](2.6.3.md)   
 - 2.7 [对象数组 ( Object[] ) 事件]()
 - 2.8 [org.w3c.dom.Node XML事件]()
 - 2.9 [扩展事件表示]()
 - 2.10 [更新，合并事件和对事件的版本控制]()
 - 2.11 [粗粒度表示事件]()
 - 2.12 [使用Insert Into 实例化和填充事件对象]()
 - 2.13 [不同类型事件的对比]()
* 3.处理模型
 - 3.1 [介绍]()
 - 3.2 [Insert 流]()
 - 3.3 [Insert & Remove 流]()
 - 3.4 [过滤器 & Where子句]()
 - 3.5 [时间窗口]()
  - 3.5.1 [时间窗口]()
  - 3.5.2 [时间批处理]()
 - 3.6 [批处理窗口]()
 - 3.7 [聚合 & 分组]()
  - 3.7.1 [Insert & Remove 流]()
  - 3.7.2 [聚合 & Group-By 输出]()
 - 3.8 [事件可见性 & 当前时间]()
* 4.上下文 & 上下文分区
 - 4.1 [介绍]()
 - 4.2 [上下文声明]()
  - 4.2.1 [上下文提供的属性]()
  - 4.2.2 [键控分段上下文]()
  - 4.2.3 [哈希分段上下文]()
  - 4.2.4 [策略分段上下文]()
  - 4.2.5 [非重叠上下文]()
  - 4.2.6 [重叠上下文]()
  - 4.2.7 [上下文条件]()
 - 4.3 上下文嵌套
  - 4.3.1 [Built-In 嵌套上下文属性]()
 - 4.4 无上下文声明的分区
 - 4.5 上下文分区结束时的输出
 - 4.6 上下文 & 命名窗口
 - 4.7 特定上下文分区中的操作
* 5.EPL 参考: 子句
 - 5.1 EPL 介绍
 - 5.2 EPL 语法
  - 5.2.1 指定时间段
  - 5.2.2 使用注释
  -	5.2.3 保留关键字
  -	5.2.4 转义字符串
  -	5.2.5 数据类型
  -	5.2.6 使用常量 & 枚举类型
  -	5.2.7 Annotation
  -	5.2.8 表达式声明
  -	5.2.9 脚本声明
  -	5.2.10 引用上下文
 - 5.3 选择事件属性和事件：Select 子句
  - 5.3.1 选择所有事件属性: select*
  -	5.3.2 选择指定事件属性
  -	5.3.3 表达式
  - 5.3.4 重命名事件属性
 - 5.21 更新插入的Stream:Update IStream条件
  - 5.21.1 事件的不变性与更新