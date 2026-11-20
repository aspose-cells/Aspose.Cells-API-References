---
title: "WorkbookMetadata"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta i metadati."
type: docs
url: /it/java/com.aspose.cells/workbookmetadata/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookMetadata
```

Rappresenta i metadati.

**Example**

Il seguente esempio crea un WorkbookMetadata.

```
           MetadataOptions options = new MetadataOptions(MetadataType.DOCUMENT_PROPERTIES);
           WorkbookMetadata meta = new WorkbookMetadata("book1.xlsx", options);
           meta.getCustomDocumentProperties().add("test", "test");
           meta.save("book2.xlsx");
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WorkbookMetadata(String fileName, MetadataOptions options)](#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-) | Crea l'oggetto dei metadati. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento integrate del foglio di calcolo. |
| [getClass()](#getClass--) |  |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo. |
| [getOptions()](#getOptions--) | Ottiene le opzioni dei metadati. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [save(String fileName)](#save-java.lang.String-) | Salva i metadati modificati nel file. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookMetadata(String fileName, MetadataOptions options) {#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-}
```
public WorkbookMetadata(String fileName, MetadataOptions options)
```


Crea l'oggetto dei metadati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String |  |
| options | [MetadataOptions](../../com.aspose.cells/metadataoptions) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento integrate del foglio di calcolo.

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


Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo.

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getOptions() {#getOptions--}
```
public MetadataOptions getOptions()
```


Ottiene le opzioni dei metadati.

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


Salva i metadati modificati nel file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

