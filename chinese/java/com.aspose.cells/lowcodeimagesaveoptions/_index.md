---
title: "LowCodeImageSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "以低代码方式保存图像的选项。"
type: docs
url: /zh/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

以低代码方式保存图像的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | 用于渲染图像的选项。 |
| [getOutputFile()](#getOutputFile--) | 获取用于保存生成数据的文件（如有需要包含路径）。 |
| [getOutputStream()](#getOutputStream--) | 获取用于写入生成数据的 Stream。 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存格式。 |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | 用于保存生成图像的保存选项提供程序。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | 用于渲染图像的选项。 |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | 设置用于保存生成数据的文件（如有需要包含路径）。 |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | 设置用于写入生成数据的 Stream。 |
| [setSaveFormat(int value)](#setSaveFormat-int-) | 设置保存格式。 |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | 用于保存生成图像的保存选项提供程序。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


用于渲染图像的选项。

**Remarks**

当指定一个 [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) 实例时， [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) 将被覆盖（如果之前已经指定过）。

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
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


获取保存格式。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Remarks**

如果已指定 [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--)，设置此属性还会更改其 [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) 的值。

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


用于保存生成图像的保存选项提供程序。

**Remarks**

当指定此属性时，由此实例指定的输出（[LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) 或 [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)）将不生效。相反，每个生成图像的输出将由提供程序指定。

**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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




### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```


用于渲染图像的选项。

**Remarks**

当指定一个 [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) 实例时， [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) 将被覆盖（如果之前已经指定过）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

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


设置保存格式。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Remarks**

如果已指定 [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--)，设置此属性还会更改其 [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


用于保存生成图像的保存选项提供程序。

**Remarks**

当指定此属性时，由此实例指定的输出（[LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) 或 [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)）将不生效。相反，每个生成图像的输出将由提供程序指定。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |

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

