---
title: "ExternalLink"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作簿中的外部链接。"
type: docs
url: /zh/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

表示工作簿中的外部链接。

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | 添加外部名称。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | 表示外部链接的数据源。 |
| [getOriginalDataSource()](#getOriginalDataSource--) | 表示外部链接的存储数据源。 |
| [getPathType()](#getPathType--) | 获取此外部链接的路径类型 |
| [getType()](#getType--) | 获取外部链接的类型。 |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | 指示此外部链接是否被其他链接引用。 |
| [isVisible()](#isVisible--) | 指示此外部链接在 MS Excel 中是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | 表示外部链接的数据源。 |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | 表示外部链接的存储数据源。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


添加外部名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | java.lang.String | 外部名称的文本。如果外部名称属于工作表，则文本应为 Sheet1!Text。 |
| referTo | java.lang.String | 外部名称的 referTo。它必须是单元格或范围。 |

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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```


表示外部链接的数据源。

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


表示外部链接的存储数据源。

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


获取此外部链接的路径类型

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


获取外部链接的类型。

请参阅 [ExternalLinkType](../../com.aspose.cells/externallinktype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```


指示此外部链接是否被其他链接引用。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


指示此外部链接在 MS Excel 中是否可见。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```


表示外部链接的数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


表示外部链接的存储数据源。

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

