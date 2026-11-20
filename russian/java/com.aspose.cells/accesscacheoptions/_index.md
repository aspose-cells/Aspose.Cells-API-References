---
title: "AccessCacheOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры кэширования доступа к данным."
type: docs
url: /ru/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Параметры кэширования для доступа к данным. Несколько параметров можно комбинировать с помощью оператора "\|".

**Remarks**

Для некоторых функций доступ к большому набору данных требует множества повторяющихся и сложных операций, таких как поиск, вычисления и т.д., и эти операции занимают много дополнительного времени. В обычных ситуациях все зависимые данные остаются неизменными во время доступа, поэтому можно создать кэши и использовать их для повышения производительности доступа. С этой целью мы предоставляем этот API, чтобы пользователь мог указать, какой тип доступа к данным следует оптимизировать с помощью возможного механизма кэширования.

Обратите внимание, что для разных параметров может потребоваться, чтобы соответствующий набор данных был только для чтения \"read-only\". И производительность доступа к данным зависит от многих факторов, использование механизма кэширования не гарантирует улучшения производительности. В некоторых ситуациях, например когда набор данных небольшой, использование кэша может занять ещё больше времени, поскольку кэширование также требует определённого дополнительного времени.
## Поля

| Поле | Описание |
| --- | --- |
| [ALL](#ALL) | Применить все возможные оптимизации для всех видов доступа к данным в рабочей книге. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Применить возможную оптимизацию при вычислении формул. |
| [CELLS_DATA](#CELLS-DATA) | Применить возможную оптимизацию при получении значений ячеек. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Применить возможную оптимизацию при получении результатов отображения ячеек([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), и т.д.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Применить возможную оптимизацию при получении результатов форматирования условных форматов. |
| [GET_FORMULA](#GET-FORMULA) | Применить возможную оптимизацию при получении формул. |
| [NONE](#NONE) | Без кэша для любого доступа к данным. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Применить возможную оптимизацию при получении позиции и размера объекта (например, Shape). |
| [SET_FORMULA](#SET-FORMULA) | Применить возможную оптимизацию при установке формул. |
| [VALIDATION](#VALIDATION) | Применить возможную оптимизацию при получении результата проверки. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Применить все возможные оптимизации для всех видов доступа к данным в рабочей книге. Все настройки и данные не должны изменяться во время оптимизированного доступа.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Применить возможную оптимизацию при вычислении формул. Данные ячеек не должны изменяться во время оптимизированного доступа, также не должны создаваться новые объекты (Cell, Row и т.д.) (например, с помощью [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Применить возможную оптимизацию при получении значений ячеек. Данные ячеек (данные и настройки Cell, Row) не должны изменяться во время оптимизированного доступа, также не должны создаваться новые объекты Cell/Row (например, с помощью [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Применить возможную оптимизацию при получении результатов отображения ячеек([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), и т.д.). Данные ячеек и объекты, связанные со стилем (стили Cell/Row/Column, ширина столбцов и т.д.) не должны изменяться во время оптимизированного доступа.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Примените возможную оптимизацию получения результата форматирования условных форматов. Все данные и настройки, которые могут влиять на результат условных форматов (настройки условных форматов, зависимые значения ячеек и т.д.), не должны изменяться во время оптимизированного доступа.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Примените возможную оптимизацию получения формул. Все данные и настройки, которые могут влиять на выражение формулы (имя листа, текст имени, столбец таблицы и т.д.), не должны изменяться во время оптимизированного доступа.

### NONE {#NONE}
```
public static final int NONE
```


Без кэша для любого доступа к данным.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Примените возможную оптимизацию получения позиции и размера объекта (например, Shape). Настройки высоты строк и ширины столбцов не должны изменяться во время оптимизированного доступа.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Примените возможную оптимизацию установки формул. Все данные и настройки, которые могут влиять на выражение формулы (имя листа, текст имени, столбец таблицы и т.д.), не должны изменяться во время оптимизированного доступа.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Примените возможную оптимизацию получения результата проверки. Все данные и настройки, которые могут влиять на результат проверки (настройки проверки, зависимые значения ячеек и т.д.), не должны изменяться во время оптимизированного доступа.

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

