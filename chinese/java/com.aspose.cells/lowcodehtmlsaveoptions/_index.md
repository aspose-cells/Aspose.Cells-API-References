---
title: "LowCodeHtmlSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "以低代码方式保存 HTML 的选项。"
type: docs
url: /zh/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

以低代码方式保存 HTML 的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | 保存 HTML 的常规选项。 |
| [getOutputFile()](#getOutputFile--) | 获取用于保存生成数据的文件（如有需要包含路径）。 |
| [getOutputStream()](#getOutputStream--) | 获取用于写入生成数据的 Stream。 |
| [getSaveFormat()](#getSaveFormat--) | 获取电子表格的格式。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | 保存 HTML 的常规选项。 |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | 设置用于保存生成数据的文件（如有需要包含路径）。 |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | 设置用于写入生成数据的 Stream。 |
| [setSaveFormat(int value)](#setSaveFormat-int-) | 设置电子表格的格式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


保存 HTML 的常规选项。

**Remarks**

当指定一个 [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) 实例时，[getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) 将被覆盖（如果之前已指定）。

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


获取用于保存生成数据的文件（如有需要包含路径）。当将此属性设置为非 null 或非空字符串时，[getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) 将被忽略。

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


获取用于写入生成数据的 Stream。当将此属性设置为非 null 时，[getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) 将被忽略。

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


获取电子表格的格式。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Remarks**

更改此属性时，由 [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) 指定的保存格式将被忽略（如果之前已指定）。

**Returns:**
int
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




### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```


保存 HTML 的常规选项。

**Remarks**

当指定一个 [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) 实例时，[getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) 将被覆盖（如果之前已指定）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


设置用于保存生成数据的文件（如有需要包含路径）。当将此属性设置为非 null 或非空字符串时，[getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) 将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


设置用于写入生成数据的 Stream。当将此属性设置为非 null 时，[getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) 将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


设置电子表格的格式。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Remarks**

更改此属性时，由 [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) 指定的保存格式将被忽略（如果之前已指定）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

