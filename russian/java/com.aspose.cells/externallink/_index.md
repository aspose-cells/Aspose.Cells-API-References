---
title: "ExternalLink"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет внешнюю ссылку в книге."
type: docs
url: /ru/java/com.aspose.cells/externallink/
---

**Inheritance:**
java.lang.Object
```
public class ExternalLink
```

Представляет внешнюю ссылку в книге.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Get External Link 
         ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
 
         //Change External Link's Data Source
         externalLink.setDataSource("d:\\link.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Добавляет внешнее имя. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Представляет источник данных внешней ссылки. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Представляет сохранённый источник данных внешней ссылки. |
| [getPathType()](#getPathType--) | Получить тип пути этой внешней ссылки |
| [getType()](#getType--) | Получает тип внешней ссылки. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Указывает, ссылаются ли другие элементы на эту внешнюю ссылку. |
| [isVisible()](#isVisible--) | Указывает, видима ли эта внешняя ссылка в MS Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Представляет источник данных внешней ссылки. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Представляет сохранённый источник данных внешней ссылки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```


Добавляет внешнее имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | java.lang.String | Текст внешнего имени. Если внешнее имя относится к листу, текст должен быть в виде Sheet1!Text. |
| referTo | java.lang.String | Значение referTo внешнего имени. Оно должно быть ячейкой или диапазоном. |

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


Представляет источник данных внешней ссылки.

**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```


Представляет сохранённый источник данных внешней ссылки.

**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```


Получить тип пути этой внешней ссылки

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Получает тип внешней ссылки.

Смотрите [ExternalLinkType](../../com.aspose.cells/externallinktype).

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


Указывает, ссылаются ли другие элементы на эту внешнюю ссылку.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Указывает, видима ли эта внешняя ссылка в MS Excel.

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


Представляет источник данных внешней ссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```


Представляет сохранённый источник данных внешней ссылки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

