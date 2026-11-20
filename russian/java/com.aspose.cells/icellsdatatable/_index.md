---
title: "ICellsDataTable"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет таблицу данных."
type: docs
url: /ru/java/com.aspose.cells/icellsdatatable/
---
```
public interface ICellsDataTable
```

Представляет таблицу данных.

**Remarks**
## Методы

| Метод | Описание |
| --- | --- |
| [beforeFirst()](#beforeFirst--) | Переместите курсор в начало этого объекта, непосредственно перед первой строкой. |
| [get(int columnIndex)](#get-int-) | Получает данные, хранящиеся в столбце, указанном по индексу. |
| [get(String columnName)](#get-java.lang.String-) | Получает данные, хранящиеся в столбце, указанном по имени столбца. |
| [getColumns()](#getColumns--) | Получает имя столбцов. |
| [getCount()](#getCount--) | Получает количество записей. -1 означает неизвестное количество записей. |
| [next()](#next--) | Перемещает курсор вниз на одну строку от текущей позиции. |
### beforeFirst() {#beforeFirst--}
```
public abstract void beforeFirst()
```


Переместите курсор в начало этого объекта, непосредственно перед первой строкой.

### get(int columnIndex) {#get-int-}
```
public abstract Object get(int columnIndex)
```


Получает данные, хранящиеся в столбце, указанном по индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnIndex | int | Нулевой индекс столбца. |

**Returns:**
java.lang.Object - 
### get(String columnName) {#get-java.lang.String-}
```
public abstract Object get(String columnName)
```


Получает данные, хранящиеся в столбце, указанном по имени столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| columnName | java.lang.String | Имя столбца. |

**Returns:**
java.lang.Object - 
### getColumns() {#getColumns--}
```
public abstract String[] getColumns()
```


Получает имя столбцов.

**Returns:**
java.lang.String[]
### getCount() {#getCount--}
```
public abstract int getCount()
```


Получает количество записей. -1 означает неизвестное количество записей.

**Returns:**
int
### next() {#next--}
```
public abstract boolean next()
```


Перемещает курсор вниз на одну строку от текущей позиции.

**Returns:**
boolean - если новая текущая строка действительна; false, если строк больше нет
