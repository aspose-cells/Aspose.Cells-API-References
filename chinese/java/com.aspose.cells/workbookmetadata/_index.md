---
title: "WorkbookMetadata"
second_title: "Aspose.Cells for Java API 参考"
description: "表示元数据。"
type: docs
url: /zh/java/com.aspose.cells/workbookmetadata/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookMetadata
```

表示元数据。

**Example**

以下示例创建一个 WorkbookMetadata。

```
           MetadataOptions options = new MetadataOptions(MetadataType.DOCUMENT_PROPERTIES);
           WorkbookMetadata meta = new WorkbookMetadata("book1.xlsx", options);
           meta.getCustomDocumentProperties().add("test", "test");
           meta.save("book2.xlsx");
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WorkbookMetadata(String fileName, MetadataOptions options)](#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-) | 创建元数据对象。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | 返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有内置文档属性。 |
| [getClass()](#getClass--) |  |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | 返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有自定义文档属性。 |
| [getOptions()](#getOptions--) | 获取元数据的选项。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [save(String fileName)](#save-java.lang.String-) | 将修改后的元数据保存到文件。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookMetadata(String fileName, MetadataOptions options) {#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-}
```
public WorkbookMetadata(String fileName, MetadataOptions options)
```


创建元数据对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String |  |
| options | [MetadataOptions](../../com.aspose.cells/metadataoptions) |  |

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
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有内置文档属性。

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有自定义文档属性。

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getOptions() {#getOptions--}
```
public MetadataOptions getOptions()
```


获取元数据的选项。

**Returns:**
[MetadataOptions](../../com.aspose.cells/metadataoptions)
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




### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


将修改后的元数据保存到文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件名。 |

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

