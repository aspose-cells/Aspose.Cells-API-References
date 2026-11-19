---
title: "SpreadsheetLocker"
second_title: "Aspose.Cells for Java API 参考"
description: "用于锁定电子表格文件的低代码 API。"
type: docs
url: /zh/java/com.aspose.cells/spreadsheetlocker/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetLocker
```

用于锁定电子表格文件的低代码 API。

**Example**

```
         SpreadsheetLocker.process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-) | 使用指定设置锁定电子表格文件。 |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-) | 使用指定设置锁定电子表格文件。 |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-) | 使用指定设置锁定电子表格文件。 |
| [process(String templateFile, String resultFile, String openPassword, String writePassword)](#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | 使用指定设置锁定电子表格文件。 |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)
```


使用指定设置锁定电子表格文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | 输入和加载的选项。 |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 输出和保存的选项。 |
| provider | [AbstractLowCodeProtectionProvider](../../com.aspose.cells/abstractlowcodeprotectionprovider) | 提供保护设置的实现 |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)
```


使用指定设置锁定电子表格文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | 输入和加载的选项。 |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 输出和保存的选项。 |
| openPassword | java.lang.String | 文件加密密码 |
| writePassword | java.lang.String | 用于保护修改电子表格的密码 |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)
```


使用指定设置锁定电子表格文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | 输入和加载的选项。 |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 输出和保存的选项。 |
| openPassword | java.lang.String | 文件加密密码 |
| writePassword | java.lang.String | 用于保护修改电子表格的密码 |
| workbookPassword | java.lang.String | 用于保护工作簿的密码 |
| workbookType | int | [ProtectionType](../../com.aspose.cells/protectiontype)。用于保护工作簿的保护类型 |

### process(String templateFile, String resultFile, String openPassword, String writePassword) {#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile, String openPassword, String writePassword)
```


使用指定设置锁定电子表格文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| templateFile | java.lang.String | 要锁定的模板文件 |
| resultFile | java.lang.String | 生成的文件。 |
| openPassword | java.lang.String | 文件加密密码 |
| writePassword | java.lang.String | 用于保护修改电子表格的密码 |

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

