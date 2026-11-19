---
title: "ImageConverter"
second_title: "Aspose.Cells for Java API 参考"
description: "用于将模板文件转换为图像的转换器。"
type: docs
url: /zh/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

用于将模板文件转换为图像的转换器。

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | 将模板文件转换为图像 |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | 将模板文件转换为图像 |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | 将模板文件转换为图像。 |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```


将模板文件转换为图像

**Remarks**

在将支持多页的图像格式（例如 tiff）转换为图像时，指定的 [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) 或 [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) 将直接用于生成的图像。

对于其他类型的图像，如果保存选项已指定 Stream 作为输出，则所有生成的图像都将保存到同一 Stream。否则，输出文件将根据保存选项中指定的输出文件，通过在文件名后附加工作表的序号和拆分部分来构建。例如，如果指定的输出文件为 Image.png，则生成的图像文件将为 Image\_0\_0.png、Image\_0\_1.png、...、Image\_1\_0.png、...

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | 输入和加载的选项。 |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 输出和保存的选项。 |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


将模板文件转换为图像

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | 输入和加载的选项。 |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 保存选项。其输出（[LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) 或 [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)）无效，因为所有输出都将由 \"provider\" 参数指定。 |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | 用于保存生成图像的保存选项提供者 |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


将模板文件转换为图像。

**Remarks**

输出文件将根据指定的结果文件，通过在文件名后附加工作表的序号和拆分部分来构建。例如，如果指定的输出文件为 Image.png，则生成的图像文件将为 Image\_0\_0.png、Image\_0\_1.png、...、Image\_1\_0.png、...

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | java.lang.String | 要转换为图像的模板文件。 |
| resultFile | java.lang.String | 生成图像的结果文件（名称模式）。 |

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

