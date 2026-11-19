---
title: "TextConverter"
second_title: "Aspose.Cells for Java API 参考"
description: "用于在基于文本的格式 csv、tsv、dif... 与其他电子表格文件格式之间进行转换的转换器。"
type: docs
url: /zh/java/com.aspose.cells/textconverter/
---

**Inheritance:**
java.lang.Object
```
public class TextConverter
```

用于在基于文本的格式（csv、tsv、dif...）与其他电子表格文件格式之间转换的转换器。

**Example**

```
         TextConverter.process("template.csv", "res.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | 在基于文本的格式和其他电子表格文件格式之间转换文件格式。 |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | 在基于文本的文件和其他格式之间转换给定的模板文件。 |
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


在基于文本的格式和其他电子表格文件格式之间转换文件格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | 输入和加载的选项。 |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 输出和保存的选项。 |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


在基于文本的文件和其他格式之间转换给定的模板文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | java.lang.String | 待转换的模板文件。 |
| resultFile | java.lang.String | 生成的文件。 |

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

