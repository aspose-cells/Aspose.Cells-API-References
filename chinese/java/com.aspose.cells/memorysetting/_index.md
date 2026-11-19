---
title: "MemorySetting"
second_title: "Aspose.Cells for Java API 参考"
description: "单元格数据模型的内存使用模式。"
type: docs
url: /zh/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

单元格数据模型的内存使用模式。
## 字段

| 字段 | 描述 |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | 更倾向于内存性能，并使用文件而非内存来维护单元格数据。 |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | 更倾向于内存性能。 |
| [NORMAL](#NORMAL) | 单元格模型的默认模式。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```


更倾向于内存性能，并使用文件而非内存来维护单元格数据。

**Remarks**

在此模式下，单元格数据将以紧凑格式维护，主要数据将保存在临时文件而非内存中。因此，与[MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE)模式相比，此模式可能进一步降低内存消耗，但访问单元格数据的 IO 操作也会导致更高的时间成本。

此选项自 v25.7.0 起可用。

| 使用此模式时的一些显著限制和推荐操作： |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 当在同一工作簿的任何工作表中使用此模式时，应在工作结束时调用[Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--)以释放所有资源，例如临时文件。 |
| 随机访问单元格会导致性能较差，因为数据需要随机且重复读取（因此文件指针会相应改变，需要反复进行 IO 操作）。如果可能，请始终按顺序（逐行）访问数据。 |
| 当一行/单元格的数据被更改时，其他单元格/行的数据也可能受到影响（例如数据会被移动/移位到其他位置以为更改后的数据分配足够的空间）。因此，每一次数据的更改都需要同步其他已有对象（如 Row 或 Cell 对象）。为获得更佳性能，请不要同时维护多个 Row/Cell。逐个处理它们可以减少数据同步，从而提升性能。 |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


更倾向于内存性能。

**Remarks**

使用此模式时，单元格数据将以紧凑格式保存，以降低内存消耗。另一方面，紧凑数据可能导致更高的时间成本，尤其是在更新单元格数据或随机访问时。

此选项自 v8.0.0 起可用。

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


单元格模型的默认模式。

**Remarks**

此模式适用于所有版本。

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

