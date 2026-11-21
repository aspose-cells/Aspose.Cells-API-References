---
title: "WorkbookMetadata"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa los metadatos."
type: docs
url: /es/java/com.aspose.cells/workbookmetadata/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookMetadata
```

Representa los metadatos.

**Example**

El siguiente ejemplo crea un WorkbookMetadata.

```
           MetadataOptions options = new MetadataOptions(MetadataType.DOCUMENT_PROPERTIES);
           WorkbookMetadata meta = new WorkbookMetadata("book1.xlsx", options);
           meta.getCustomDocumentProperties().add("test", "test");
           meta.save("book2.xlsx");
```
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WorkbookMetadata(String fileName, MetadataOptions options)](#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-) | Cree el objeto de metadatos. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento incorporadas de la hoja de cálculo. |
| [getClass()](#getClass--) |  |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento personalizadas de la hoja de cálculo. |
| [getOptions()](#getOptions--) | Obtiene las opciones de los metadatos. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [save(String fileName)](#save-java.lang.String-) | Guarde los metadatos modificados en el archivo. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookMetadata(String fileName, MetadataOptions options) {#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-}
```
public WorkbookMetadata(String fileName, MetadataOptions options)
```


Cree el objeto de metadatos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String |  |
| options | [MetadataOptions](../../com.aspose.cells/metadataoptions) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento incorporadas de la hoja de cálculo.

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


Devuelve una colección de [DocumentProperty](../../com.aspose.cells/documentproperty) que representa todas las propiedades de documento personalizadas de la hoja de cálculo.

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getOptions() {#getOptions--}
```
public MetadataOptions getOptions()
```


Obtiene las opciones de los metadatos.

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


Guarde los metadatos modificados en el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre del archivo. |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

