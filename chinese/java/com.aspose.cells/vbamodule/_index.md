---
title: "VbaModule"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 VBA 项目中的模块。"
type: docs
url: /zh/java/com.aspose.cells/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public class VbaModule
```

表示 VBA 项目中的模块。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         int index = vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         // Get vba module
         VbaModule vbaModule = vbaProject.getModules().get(index);
         // Set codes
         vbaModule.setCodes("Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBinaryCodes()](#getBinaryCodes--) | 获取模块的二进制代码。 |
| [getClass()](#getClass--) |  |
| [getCodes()](#getCodes--) | 获取模块的代码。 |
| [getName()](#getName--) | 获取模块的名称。 |
| [getType()](#getType--) | 获取模块的类型。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCodes(String value)](#setCodes-java.lang.String-) | 设置模块的代码。 |
| [setName(String value)](#setName-java.lang.String-) | 设置模块的名称。 |
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
### getBinaryCodes() {#getBinaryCodes--}
```
public byte[] getBinaryCodes()
```


获取模块的二进制代码。

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodes() {#getCodes--}
```
public String getCodes()
```


获取模块的代码。

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


获取模块的名称。

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


获取模块的类型。

参见 [VbaModuleType](../../com.aspose.cells/vbamoduletype)。

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




### setCodes(String value) {#setCodes-java.lang.String-}
```
public void setCodes(String value)
```


设置模块的代码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置模块的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

