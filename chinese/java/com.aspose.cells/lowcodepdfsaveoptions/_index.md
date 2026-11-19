---
title: "LowCodePdfSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "以低代码方式保存 PDF 的选项。"
type: docs
url: /zh/java/com.aspose.cells/lowcodepdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodePdfSaveOptions extends LowCodeSaveOptions
```

以低代码方式保存 PDF 的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LowCodePdfSaveOptions()](#LowCodePdfSaveOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | 获取用于保存生成数据的文件（如有需要包含路径）。 |
| [getOutputStream()](#getOutputStream--) | 获取用于写入生成数据的 Stream。 |
| [getPdfOptions()](#getPdfOptions--) | 用于保存 PDF 文件的选项。 |
| [getSaveFormat()](#getSaveFormat--) | 输出的保存格式。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | 设置用于保存生成数据的文件（如有需要包含路径）。 |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | 设置用于写入生成数据的 Stream。 |
| [setPdfOptions(PdfSaveOptions value)](#setPdfOptions-com.aspose.cells.PdfSaveOptions-) | 用于保存 PDF 文件的选项。 |
| [setSaveFormat(int value)](#setSaveFormat-int-) | 输出的保存格式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodePdfSaveOptions() {#LowCodePdfSaveOptions--}
```
public LowCodePdfSaveOptions()
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
### getPdfOptions() {#getPdfOptions--}
```
public PdfSaveOptions getPdfOptions()
```


用于保存 PDF 文件的选项。

**Returns:**
[PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


输出的保存格式。若转换为 PDF，只能使用 [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF)。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

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

### setPdfOptions(PdfSaveOptions value) {#setPdfOptions-com.aspose.cells.PdfSaveOptions-}
```
public void setPdfOptions(PdfSaveOptions value)
```


用于保存 PDF 文件的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions) |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


输出的保存格式。若转换为 PDF，只能使用 [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF)。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

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

