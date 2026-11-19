---
title: "VbaProjectReference"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 VBA 项目的引用。"
type: docs
url: /zh/java/com.aspose.cells/vbaprojectreference/
---

**Inheritance:**
java.lang.Object
```
public class VbaProjectReference
```

表示 VBA 项目的引用。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [copy(VbaProjectReference source)](#copy-com.aspose.cells.VbaProjectReference-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getExtendedLibid()](#getExtendedLibid--) | 获取引用的扩展 Libid。 |
| [getLibid()](#getLibid--) | 获取引用的 Libid。 |
| [getName()](#getName--) | 获取引用的名称。 |
| [getRelativeLibid()](#getRelativeLibid--) | 获取带相对路径的被引用 VBA 项目的标识符。 |
| [getTwiddledlibid()](#getTwiddledlibid--) | 获取引用的扭曲 Libid。 |
| [getType()](#getType--) | 获取此引用的类型。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setExtendedLibid(String value)](#setExtendedLibid-java.lang.String-) | 设置引用的扩展 Libid。 |
| [setLibid(String value)](#setLibid-java.lang.String-) | 设置引用的 Libid。 |
| [setName(String value)](#setName-java.lang.String-) | 设置引用的名称。 |
| [setRelativeLibid(String value)](#setRelativeLibid-java.lang.String-) | 设置带相对路径的被引用 VBA 项目的标识符。 |
| [setTwiddledlibid(String value)](#setTwiddledlibid-java.lang.String-) | 设置引用的扭曲 Libid。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(VbaProjectReference source) {#copy-com.aspose.cells.VbaProjectReference-}
```
public void copy(VbaProjectReference source)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [VbaProjectReference](../../com.aspose.cells/vbaprojectreference) |  |

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
### getExtendedLibid() {#getExtendedLibid--}
```
public String getExtendedLibid()
```


获取引用的扩展 Libid。

**Remarks**

仅用于控件引用。

**Returns:**
java.lang.String
### getLibid() {#getLibid--}
```
public String getLibid()
```


获取引用的 Libid。

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


获取引用的名称。

**Returns:**
java.lang.String
### getRelativeLibid() {#getRelativeLibid--}
```
public String getRelativeLibid()
```


获取带相对路径的被引用 VBA 项目的标识符。

**Remarks**

仅用于项目引用。

**Returns:**
java.lang.String
### getTwiddledlibid() {#getTwiddledlibid--}
```
public String getTwiddledlibid()
```


获取引用的扭曲 Libid。

**Remarks**

仅用于控件引用。

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


获取此引用的类型。

参见 [VbaProjectReferenceType](../../com.aspose.cells/vbaprojectreferencetype)。

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




### setExtendedLibid(String value) {#setExtendedLibid-java.lang.String-}
```
public void setExtendedLibid(String value)
```


设置引用的扩展 Libid。

**Remarks**

仅用于控件引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLibid(String value) {#setLibid-java.lang.String-}
```
public void setLibid(String value)
```


设置引用的 Libid。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置引用的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setRelativeLibid(String value) {#setRelativeLibid-java.lang.String-}
```
public void setRelativeLibid(String value)
```


设置带相对路径的被引用 VBA 项目的标识符。

**Remarks**

仅用于项目引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTwiddledlibid(String value) {#setTwiddledlibid-java.lang.String-}
```
public void setTwiddledlibid(String value)
```


设置引用的扭曲 Libid。

**Remarks**

仅用于控件引用。

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

