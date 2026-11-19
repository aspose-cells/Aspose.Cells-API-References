---
title: "SpreadsheetSplitter"
second_title: "Aspose.Cells for Java API 参考"
description: "将电子表格文件拆分为多个部分。"
type: docs
url: /zh/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

将电子表格文件拆分为多个部分。

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | 将电子表格文件拆分为多个部分。 |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | 将给定的模板文件拆分为多个部分。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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




### process(LowCodeSplitOptions options) {#process-com.aspose.cells.LowCodeSplitOptions-}
```
public static void process(LowCodeSplitOptions options)
```


将电子表格文件拆分为多个部分。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | 拆分电子表格的选项 |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


将给定的模板文件拆分为多个部分。

**Remarks**

输出文件将基于指定的生成文件，通过附加工作表序号和拆分部分序号来构建。例如，如果指定的输出文件为 Split.xlsx，则生成的文件将是 Split\_0\_0.xlsx、Split\_0\_1.xlsx、……、Split\_1\_0.xlsx、……

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | java.lang.String | 要拆分的模板文件 |
| resultFile | java.lang.String | 生成的文件（名称模式） |

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

