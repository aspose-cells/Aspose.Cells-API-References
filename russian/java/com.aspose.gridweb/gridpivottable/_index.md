---
title: "GridPivotTable"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет отчет PivotTable на листе."
type: docs
url: /ru/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

Представляет отчет PivotTable на листе. Объект PivotTable является членом коллекции [GridPivotTable](../../com.aspose.gridweb/gridpivottable). Коллекция PivotTables содержит все объекты PivotTable в элементе управления.
## Методы

| Метод | Описание |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Добавляет поле в определённую область. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Добавляет поле в определённую область. |
| [calculateData()](#calculateData--) | Вычисляет данные pivottable в ячейки. |
| [clearAllFields()](#clearAllFields--) | Очистить все поля сводной таблицы. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Получает конкретные поля по типу поля. |
| [fields(String fieldName)](#fields-java.lang.String-) | Получает конкретное поле по имени поля. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Обновляет данные и настройки pivottable из его источника данных. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Добавляет поле в определённую область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Тип области полей. |
| baseFieldIndex | int | Индекс поля в базовых полях. |

**Returns:**
int — позиция поля в конкретных полях.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Добавляет поле в определённую область.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Тип области полей. |
| fieldName | java.lang.String | Имя в базовых полях. |

**Returns:**
int — позиция поля в конкретных полях. Если поле с таким именем отсутствует, вернуть -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Вычисляет данные pivottable в ячейки.

**Remarks**

Cell.Value в диапазоне сводной таблицы может не возвращать правильный результат, если метод не был вызван. Этот метод вычисляет данные с внутренним кэшем сводной таблицы, а не из оригинального источника данных. Поэтому, если источник данных изменён, пожалуйста, сначала вызовите метод RefreshData().

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


Очистить все поля сводной таблицы.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


Получает конкретные поля по типу поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). тип поля. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


Получает конкретное поле по имени поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldName | java.lang.String | имя поля. |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### refreshData() {#refreshData--}
```
public void refreshData()
```


Обновляет данные и настройки pivottable из его источника данных.

**Remarks**

Мы соберём данные из источника данных в кэш сводной таблицы, затем вычислим данные из кэша в ячейки. Этот метод используется только для сбора всех данных в кэш сводной таблицы.

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

