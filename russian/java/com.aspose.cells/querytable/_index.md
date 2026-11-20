---
title: "QueryTable"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет информацию о QueryTable."
type: docs
url: /ru/java/com.aspose.cells/querytable/
---

**Inheritance:**
java.lang.Object
```
public class QueryTable
```

Представляет информацию о QueryTable.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Getting the first query table in the worksheet if exists
         //QueryTable qt = worksheet.QueryTables[0];
         //Getting display address of the query table.
         //string address = qt.ResultRange.Address;
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdjustColumnWidth()](#getAdjustColumnWidth--) | Возвращает или задаёт свойство AdjustColumnWidth объекта. |
| [getClass()](#getClass--) |  |
| [getConnectionId()](#getConnectionId--) | Получает идентификатор соединения запросной таблицы. |
| [getExternalConnection()](#getExternalConnection--) | Получает связанное внешнее соединение. |
| [getName()](#getName--) | Получает имя запросной таблицы. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Возвращает или задаёт свойство PreserveFormatting объекта. |
| [getResultRange()](#getResultRange--) | Получает диапазон результата. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdjustColumnWidth(boolean value)](#setAdjustColumnWidth-boolean-) | Возвращает или задаёт свойство AdjustColumnWidth объекта. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Возвращает или задаёт свойство PreserveFormatting объекта. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAdjustColumnWidth() {#getAdjustColumnWidth--}
```
public boolean getAdjustColumnWidth()
```


Возвращает или задаёт свойство AdjustColumnWidth объекта.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```


Получает идентификатор соединения запросной таблицы.

**Returns:**
int
### getExternalConnection() {#getExternalConnection--}
```
public ExternalConnection getExternalConnection()
```


Получает связанное внешнее соединение.

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getName() {#getName--}
```
public String getName()
```


Получает имя запросной таблицы.

**Returns:**
java.lang.String
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```


Возвращает или задаёт свойство PreserveFormatting объекта.

**Returns:**
boolean
### getResultRange() {#getResultRange--}
```
public Range getResultRange()
```


Получает диапазон результата.

**Returns:**
[Range](../../com.aspose.cells/range) - 
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




### setAdjustColumnWidth(boolean value) {#setAdjustColumnWidth-boolean-}
```
public void setAdjustColumnWidth(boolean value)
```


Возвращает или задаёт свойство AdjustColumnWidth объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```


Возвращает или задаёт свойство PreserveFormatting объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

