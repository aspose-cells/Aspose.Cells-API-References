---
title: "ErrorCheckType"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все типы проверки ошибок."
type: docs
url: /ru/java/com.aspose.cells/errorchecktype/
---

**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```

Представляет все типы проверки ошибок.
## Поля

| Поле | Описание |
| --- | --- |
| [CALC](#CALC) | **Примечания** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | Игнорировать ошибки, когда ячейки содержат значение, отличное от вычисленной формулы столбца. |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | Игнорировать ошибки, когда формулы ссылаются на пустые ячейки. |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | Игнорировать ошибки, когда ячейки содержат формулы, приводящие к ошибке. |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | Игнорировать ошибки, когда формула в области вашего листа отличается от других формул в той же области. |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | Игнорировать ошибки, когда формулы пропускают определённые ячейки в области. |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | Игнорировать ошибки, когда числа отформатированы как текст или предваряются апострофом |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | Игнорировать ошибки, когда значение ячейки в таблице не соответствует указанным правилам проверки данных. |
| [TEXT_DATE](#TEXT-DATE) | Игнорировать ошибки, когда формулы содержат ячейки, отформатированные как текст, с годами, представленными двумя цифрами. |
| [TEXT_NUMBER](#TEXT-NUMBER) | Игнорировать ошибки, когда числа отформатированы как текст или предваряются апострофом |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | Игнорировать ошибки, когда формулы содержат ячейки, отформатированные как текст, с годами, представленными двумя цифрами. |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | Игнорировать ошибки, когда разблокированные ячейки содержат формулы. |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | Игнорировать ошибки, когда разблокированные ячейки содержат формулы. |
| [VALIDATION](#VALIDATION) | Игнорировать ошибки, когда значение ячейки в таблице не соответствует указанным правилам проверки данных. |
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
### CALC {#CALC}
```
public static final int CALC
```


**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте перечисление ErrorCheckType.EvaluationError. Этот метод будет удалён через 12 месяцев, начиная с октября 2023 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```


Игнорировать ошибки, когда ячейки содержат значение, отличное от вычисленной формулы столбца.

### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```


Игнорировать ошибки, когда формулы ссылаются на пустые ячейки.

### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```


Игнорировать ошибки, когда ячейки содержат формулы, приводящие к ошибке.

### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```


Игнорировать ошибки, когда формула в области вашего листа отличается от других формул в той же области.

### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```


Игнорировать ошибки, когда формулы пропускают определённые ячейки в области.

### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```


Игнорировать ошибки, когда числа отформатированы как текст или предваряются апострофом

### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```


Игнорировать ошибки, когда значение ячейки в таблице не соответствует указанным правилам проверки данных.

### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```


Игнорировать ошибки, когда формулы содержат ячейки, отформатированные как текст, с годами, представленными двумя цифрами.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте перечисление ErrorCheckType.TwoDigitTextYear. Этот метод будет удалён через 12 месяцев, начиная с октября 2023 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```


Игнорировать ошибки, когда числа отформатированы как текст или предваряются апострофом

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте перечисление ErrorCheckType.NumberStoredAsText. Этот метод будет удалён через 12 месяцев, начиная с октября 2023 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```


Игнорировать ошибки, когда формулы содержат ячейки, отформатированные как текст, с годами, представленными двумя цифрами.

### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```


Игнорировать ошибки, когда разблокированные ячейки содержат формулы.

### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```


Игнорировать ошибки, когда разблокированные ячейки содержат формулы.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте перечисление ErrorCheckType.UnproctedFormula. Этот метод будет удалён через 12 месяцев, начиная с октября 2023 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Игнорировать ошибки, когда значение ячейки в таблице не соответствует указанным правилам проверки данных.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте перечисление ErrorCheckType.TableDataValidation. Этот метод будет удалён через 12 месяцев, начиная с октября 2023 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

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

