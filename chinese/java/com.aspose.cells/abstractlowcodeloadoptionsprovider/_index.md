---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells for Java API 参考"
description: "实现提供多个加载选项，以用于使用多个输入（如模板文件）的过程。"
type: docs
url: /zh/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

实现提供多种加载选项，用于使用多个输入（如模板文件）的过程。

**Remarks**

例如，[SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) 功能需要多个模板文件进行合并。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | 在处理当前输入的部分后释放资源。 |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | 获取用于加载当前处理部分数据的加载选项。 |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | 检查是否还有更多输入。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


在处理当前输入的部分后释放资源。

**Remarks**

默认情况下，此方法直接关闭由 [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) 指定的流（如果加载选项将流作为来源）。用户可以覆盖此方法，以根据其需求以及 [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--) 的实现来控制资源的释放方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | 用于当前拆分部分的加载选项。 |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```


获取用于加载当前处理部分数据的加载选项。

**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```


检查是否还有更多输入。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

