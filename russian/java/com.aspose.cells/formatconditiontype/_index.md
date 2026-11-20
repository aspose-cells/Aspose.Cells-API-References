---
title: "FormatConditionType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Тип правила условного форматирования."
type: docs
url: /ru/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

Тип правила условного форматирования.
## Поля

| Поле | Описание |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | Это правило условного форматирования выделяет ячейки, значения которых выше или ниже среднего для всех значений в диапазоне. |
| [BEGINS_WITH](#BEGINS-WITH) | Это правило условного форматирования выделяет ячейки в диапазоне, которые начинаются с заданного текста. |
| [CELL_VALUE](#CELL-VALUE) | Это правило условного форматирования сравнивает значение ячейки с результатом, вычисленным формулой, используя оператор. |
| [COLOR_SCALE](#COLOR-SCALE) | Это правило условного форматирования создает градуированную цветовую шкалу в ячейках. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | Это правило условного форматирования выделяет ячейки, которые полностью пусты. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | Это правило условного форматирования выделяет ячейки с ошибками формул. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | Это правило условного форматирования выделяет ячейки, содержащие заданный текст. |
| [DATA_BAR](#DATA-BAR) | Это правило условного форматирования отображает градуированную полосу данных в диапазоне ячеек. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | Это правило условного форматирования выделяет дублированные значения. |
| [ENDS_WITH](#ENDS-WITH) | Это правило условного форматирования выделяет ячейки, заканчивающиеся заданным текстом. |
| [EXPRESSION](#EXPRESSION) | Это правило условного форматирования содержит формулу для вычисления. |
| [ICON_SET](#ICON-SET) | Это правило условного форматирования применяет значки к ячейкам в соответствии с их значениями. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | Это правило условного форматирования выделяет ячейки, которые не пусты. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | Это правило условного форматирования выделяет ячейки без ошибок формул. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | Это правило условного форматирования выделяет ячейки, которые не содержат заданный текст. |
| [TIME_PERIOD](#TIME-PERIOD) | Это правило условного форматирования выделяет ячейки, содержащие даты в указанном временном периоде. |
| [TOP_10](#TOP-10) | Это правило условного форматирования выделяет ячейки, значения которых попадают в верхний N или нижний N диапазон, как указано. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | Это правило условного форматирования выделяет уникальные значения в диапазоне. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


Это правило условного форматирования выделяет ячейки, значения которых выше или ниже среднего для всех значений в диапазоне.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


Это правило условного форматирования выделяет ячейки в диапазоне, которые начинаются с заданного текста. Эквивалентно использованию функции листа LEFT() и сравнению значений.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Это правило условного форматирования сравнивает значение ячейки с результатом, вычисленным формулой, используя оператор.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


Это правило условного форматирования создает градуированную цветовую шкалу в ячейках.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


Это правило условного форматирования выделяет ячейки, которые полностью пусты. Эквивалентно использованию LEN(TRIM()). Это означает, что если ячейка содержит только символы, которые удалит TRIM(), то она считается пустой. Пустая ячейка также считается пустой.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


Это правило условного форматирования выделяет ячейки с ошибками формул. Эквивалентно использованию функции листа ISERROR() для определения наличия ошибки формулы.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


Это правило условного форматирования выделяет ячейки, содержащие заданный текст. Эквивалентно использованию функции листа SEARCH() для определения, содержит ли ячейка данный текст.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


Это правило условного форматирования отображает градуированную полосу данных в диапазоне ячеек.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


Это правило условного форматирования выделяет дублированные значения.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


Это правило условного форматирования выделяет ячейки, заканчивающиеся заданным текстом. Эквивалентно использованию функции листа RIGHT() и сравнению значений.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


Это правило условного форматирования содержит формулу для вычисления. Когда результат формулы истинный, ячейка выделяется.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


Это правило условного форматирования применяет значки к ячейкам в соответствии с их значениями.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


Это правило условного форматирования выделяет ячейки, которые не пусты. Эквивалент использования LEN(TRIM()). Это означает, что если ячейка содержит только символы, которые удалит TRIM(), она считается пустой. Пустая ячейка также считается пустой.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


Это правило условного форматирования выделяет ячейки без ошибок формул. Эквивалент использования функции листа ISERROR() для определения наличия ошибки формулы.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


Это правило условного форматирования выделяет ячейки, не содержащие заданный текст. Эквивалент использования функции листа SEARCH() для определения, содержит ли ячейка текст или нет.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


Это правило условного форматирования выделяет ячейки, содержащие даты в указанном периоде. Оценивается базовое значение ячейки, поэтому ячейка не обязана быть отформатирована как дата для оценки. Например, если ячейка содержит значение 38913, условное форматирование будет применено, если правило требует значение 7/14/2006.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


Это правило условного форматирования выделяет ячейки, значения которых попадают в верхний N или нижний N диапазон, как указано.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


Это правило условного форматирования выделяет уникальные значения в диапазоне.

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

