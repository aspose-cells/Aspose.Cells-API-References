---
title: "AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells for Java API 参考"
description: "实现提供多种保存选项，用于需要多个输出的过程。"
type: docs
url: /zh/java/com.aspose.cells/abstractlowcodesaveoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeSaveOptionsProvider
```

实现提供多种保存选项，以满足需要多个输出的流程。例如，[SpreadsheetSplitter](../../com.aspose.cells/spreadsheetsplitter) 功能需要多个目标来保存拆分后的文件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider()](#AbstractLowCodeSaveOptionsProvider--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | 在处理当前拆分部分后释放资源。 |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | 获取用于获取当前拆分部分输出设置的保存选项。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeSaveOptionsProvider() {#AbstractLowCodeSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


在处理当前拆分部分后释放资源。

**Remarks**

默认情况下，此方法直接关闭由[LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)指定的流（如果保存选项将流作为目标）。用户可以覆盖此方法，以根据其需求以及[getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-)的实现来控制资源的释放方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 用于当前拆分部分的保存选项。 |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public abstract LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


获取用于获取当前拆分部分输出设置的保存选项。返回 null 表示跳过给定的部分。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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

