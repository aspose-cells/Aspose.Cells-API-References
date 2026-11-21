---
title: "WorkbookMetadata"
second_title: "Aspose.Cells for Java API Referansı"
description: "Meta verileri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/workbookmetadata/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookMetadata
```

Meta verileri temsil eder.

**Example**

Aşağıdaki örnek bir WorkbookMetadata oluşturur.

```
           MetadataOptions options = new MetadataOptions(MetadataType.DOCUMENT_PROPERTIES);
           WorkbookMetadata meta = new WorkbookMetadata("book1.xlsx", options);
           meta.getCustomDocumentProperties().add("test", "test");
           meta.save("book2.xlsx");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WorkbookMetadata(String fileName, MetadataOptions options)](#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-) | Meta veri nesnesini oluştur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm yerleşik belge özelliklerini temsil eder. |
| [getClass()](#getClass--) |  |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm özel belge özelliklerini temsil eder. |
| [getOptions()](#getOptions--) | Meta verinin seçeneklerini al. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [save(String fileName)](#save-java.lang.String-) | Değiştirilmiş meta veriyi dosyaya kaydet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookMetadata(String fileName, MetadataOptions options) {#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-}
```
public WorkbookMetadata(String fileName, MetadataOptions options)
```


Meta veri nesnesini oluştur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String |  |
| options | [MetadataOptions](../../com.aspose.cells/metadataoptions) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm yerleşik belge özelliklerini temsil eder.

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


Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm özel belge özelliklerini temsil eder.

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getOptions() {#getOptions--}
```
public MetadataOptions getOptions()
```


Meta verinin seçeneklerini al.

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


Değiştirilmiş meta veriyi dosyaya kaydet.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosya adı. |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

