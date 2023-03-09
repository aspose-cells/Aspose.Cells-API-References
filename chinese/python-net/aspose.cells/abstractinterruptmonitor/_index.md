---
title: AbstractInterruptMonitor类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells/abstractinterruptmonitor/
is_root: false
---
## AbstractInterruptMonitor类
监控所有耗时操作中的中断请求。



AbstractInterruptMonitor 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_interruption_requested](/cells/zh/python-net/aspose.cells/abstractinterruptmonitor/is_interruption_requested) |指示当前操作是否请求中断。<br/>如果为真，则当前操作将被中断。<br/>实现应该在这里进行快速高效的检查，否则可能成为程序的另一个瓶颈。|
| [terminate_without_exception](/cells/zh/python-net/aspose.cells/abstractinterruptmonitor/terminate_without_exception) |当程序被中断时，是安静地终止程序还是抛出异常。<br/>默认为false，即[AbstractInterruptMonitor.is_interruption_requested](/cells/zh/python-net/aspose.cells/abstractinterruptmonitor#is_interruption_requested)为true时，<br/>将抛出代码为 [ExceptionType.INTERRUPTED](/cells/zh/python-net/aspose.cells/exceptiontype#INTERRUPTED) 的 [CellsException](/cells/zh/python-net/aspose.cells/cellsexception)。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [CellsException](/cells/zh/python-net/aspose.cells/cellsexception)
