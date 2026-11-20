---
title: "WorkbookMetadata"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет метаданные."
type: docs
url: /ru/java/com.aspose.cells/workbookmetadata/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookMetadata
```

Представляет метаданные.

**Example**

В следующем примере создаётся WorkbookMetadata.

```
           MetadataOptions options = new MetadataOptions(MetadataType.DOCUMENT_PROPERTIES);
           WorkbookMetadata meta = new WorkbookMetadata("book1.xlsx", options);
           meta.getCustomDocumentProperties().add("test", "test");
           meta.save("book2.xlsx");
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [WorkbookMetadata(String fileName, MetadataOptions options)](#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-) | Создайте объект метаданных. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все встроенные свойства документа электронной таблицы. |
| [getClass()](#getClass--) |  |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все пользовательские свойства документа электронной таблицы. |
| [getOptions()](#getOptions--) | Получает параметры метаданных. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [save(String fileName)](#save-java.lang.String-) | Сохраняет изменённые метаданные в файл. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookMetadata(String fileName, MetadataOptions options) {#WorkbookMetadata-java.lang.String-com.aspose.cells.MetadataOptions-}
```
public WorkbookMetadata(String fileName, MetadataOptions options)
```


Создайте объект метаданных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String |  |
| options | [MetadataOptions](../../com.aspose.cells/metadataoptions) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все встроенные свойства документа электронной таблицы.

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


Возвращает коллекцию [DocumentProperty](../../com.aspose.cells/documentproperty), представляющую все пользовательские свойства документа электронной таблицы.

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getOptions() {#getOptions--}
```
public MetadataOptions getOptions()
```


Получает параметры метаданных.

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


Сохраняет изменённые метаданные в файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла. |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

