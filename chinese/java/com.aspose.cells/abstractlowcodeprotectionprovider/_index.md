---
title: "AbstractLowCodeProtectionProvider"
second_title: "Aspose.Cells for Java API 参考"
description: "实现提供保护设置"
type: docs
url: /zh/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

实现提供保护设置
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | 获取打开电子表格文件的密码。 |
| [getWorkbookPassword()](#getWorkbookPassword--) | 获取使用指定保护类型保护工作簿的密码。 |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | 获取用于保护工作簿的保护类型。 |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | 获取保护指定工作表的密码。 |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | 获取用于保护指定工作表的保护类型。 |
| [getWritePassword()](#getWritePassword--) | 获取修改电子表格文件的密码。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
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
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


获取打开电子表格文件的密码。

**Returns:**
java.lang.String - 打开电子表格文件的密码。空字符串表示对打开文件没有保护。
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


获取使用指定保护类型保护工作簿的密码。

**Returns:**
java.lang.String - 保护工作簿的密码。
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


获取用于保护工作簿的保护类型。

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype)。用于保护工作簿的保护类型。[ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) 表示工作簿没有保护。
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


获取保护指定工作表的密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - 保护指定工作表的密码。
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


获取用于保护指定工作表的保护类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype)。用于保护指定工作表的保护类型。[ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) 表示工作表没有保护。
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


获取修改电子表格文件的密码。

**Returns:**
java.lang.String - 修改电子表格文件的密码。空字符串表示对修改文件没有保护。
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

