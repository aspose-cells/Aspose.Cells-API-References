---
title: "FormatCondition"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет условие условного форматирования."
type: docs
url: /ru/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

Представляет условие условного форматирования.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
 
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
 
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
 
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         //Saving the Excel file
         workbook.save("output.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | Получить экземпляр "AboveAverage" условного форматирования. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | Получить экземпляр "ColorScale" условного форматирования. |
| [getDataBar()](#getDataBar--) | Получить экземпляр "DataBar" условного форматирования. |
| [getFormula1()](#getFormula1--) | Получает значение или выражение, связанное с условным форматированием. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Получает значение или выражение, связанное с этим условием форматирования. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Получает значение или выражение условного форматирования ячейки. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | Получает формулу условного форматирования ячейки. |
| [getFormula2()](#getFormula2--) | Получает значение или выражение, связанное с условным форматированием. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Получает значение или выражение, связанное с этим условием форматирования. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Получает значение или выражение условного форматирования ячейки. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | Получает формулу условного форматирования ячейки. |
| [getIconSet()](#getIconSet--) | Получить экземпляр "IconSet" условного форматирования. |
| [getOperator()](#getOperator--) | Получает тип оператора условного форматирования. |
| [getPriority()](#getPriority--) | Приоритет этого правила условного форматирования. |
| [getStopIfTrue()](#getStopIfTrue--) | True, правила с более низким приоритетом не могут применяться к этому правилу, когда это правило оценивается как true. |
| [getStyle()](#getStyle--) | Получает или задает стиль условно отформатированных диапазонов ячеек. |
| [getText()](#getText--) | Текстовое значение в правиле условного форматирования "text contains". |
| [getTimePeriod()](#getTimePeriod--) | Применимый период времени в правиле условного форматирования "date occurrin". |
| [getTop10()](#getTop10--) | Получить экземпляр "Top10" условного форматирования. |
| [getType()](#getType--) | Получает тип условного формата. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Устанавливает значение или выражение, связанное с условным форматированием. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Устанавливает значение или выражение, связанное с этим условием форматирования. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Устанавливает значение или выражение, связанное с условным форматированием. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Устанавливает значение или выражение, связанное с этим условием форматирования. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | Устанавливает значение или выражение, связанное с этим условием форматирования. |
| [setOperator(int value)](#setOperator-int-) | Устанавливает тип оператора условного формата. |
| [setPriority(int value)](#setPriority-int-) | Приоритет этого правила условного форматирования. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | True, правила с более низким приоритетом не могут применяться к этому правилу, когда это правило оценивается как true. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Получает или задает стиль условно отформатированных диапазонов ячеек. |
| [setText(String value)](#setText-java.lang.String-) | Текстовое значение в правиле условного форматирования "text contains". |
| [setTimePeriod(int value)](#setTimePeriod-int-) | Применимый период времени в правиле условного форматирования "date occurrin". |
| [setType(int value)](#setType-int-) | Устанавливает тип условного формата. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


Получить экземпляр "AboveAverage" условного форматирования. Правило экземпляра по умолчанию выделяет ячейки, значения которых выше среднего для всех значений в диапазоне. Действительно только для типа = AboveAverage.

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


Получить экземпляр "ColorScale" условного форматирования. Экземпляр по умолчанию представляет собой "green-yellow-red" 3ColorScale. Действительно только для типа = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


Получить экземпляр "DataBar" условного форматирования. Цвет экземпляра по умолчанию — синий. Действительно только для типа = DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Получает значение или выражение, связанное с условным форматированием.

**Remarks**

Пожалуйста, добавьте все области перед установкой формулы. При установке формулы для этого условия, если входное значение начинается с '=', оно будет восприниматься как формула. В противном случае оно будет восприниматься как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Получает значение или выражение, связанное с этим условием форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String — значение или выражение, связанное с этим условием форматирования.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Получает значение или выражение условного форматирования ячейки.

**Remarks**

Указанная ячейка должна быть включена в это условное форматирование, иначе будет возвращено null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String — значение или выражение, связанное с условным форматированием ячейки.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


Получает формулу условного форматирования ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String — формула.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Получает значение или выражение, связанное с условным форматированием.

**Remarks**

Пожалуйста, добавьте все области перед установкой формулы. При установке формулы для этого условия, если входное значение начинается с '=', оно будет восприниматься как формула. В противном случае оно будет восприниматься как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Получает значение или выражение, связанное с этим условием форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String — значение или выражение, связанное с этим условием форматирования.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Получает значение или выражение условного форматирования ячейки.

**Remarks**

Указанная ячейка должна быть включена в это условное форматирование, иначе будет возвращено null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String — значение или выражение, связанное с условным форматированием ячейки.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


Получает формулу условного форматирования ячейки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Индекс строки. |
| столбец | int | Индекс столбца. |

**Returns:**
java.lang.String — формула.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


Получить экземпляр "IconSet" условного форматирования. IconSetType экземпляра по умолчанию — TrafficLights31. Действительно только для типа = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


Получает тип оператора условного форматирования.

Смотрите [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


Приоритет этого правила условного форматирования. Это значение используется для определения, какое форматирование должно быть оценено и применено. Более низкие числовые значения означают более высокий приоритет по сравнению с более высокими значениями, где '1' — самый высокий приоритет.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


True, правила с более низким приоритетом не могут применяться к этому правилу, когда это правило оценивается как true. Применяется только для Excel 2007;

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Получает или задает стиль условно отформатированных диапазонов ячеек.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


Текстовое значение в правиле условного форматирования "text contains". Действительно только для типов = containsText, notContainsText, beginsWith и endsWith. Значение по умолчанию — null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


Применимый период времени в правиле условного форматирования "date occurrin". Действительно только для типа = timePeriod. Значение по умолчанию — TimePeriodType.Today.

Смотрите [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


Получить экземпляр "Top10" условного форматирования. Правило экземпляра по умолчанию выделяет ячейки, значения которых попадают в топ‑10. Действительно только для типа = Top10.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


Получает тип условного формата.

Смотрите [FormatConditionType](../../com.aspose.cells/formatconditiontype).

**Returns:**
int
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




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Устанавливает значение или выражение, связанное с условным форматированием.

**Remarks**

Пожалуйста, добавьте все области перед установкой формулы. При установке формулы для этого условия, если входное значение начинается с '=', оно будет восприниматься как формула. В противном случае оно будет восприниматься как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\\"=...\\"".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Устанавливает значение или выражение, связанное с этим условием форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Значение или выражение, связанное с этим условием форматирования. Если входное значение начинается с '=', оно будет рассматриваться как формула. В противном случае оно будет рассматриваться как обычное значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\\"=...\\"". |
| isR1C1 | boolean | Является ли формула формулой R1C1. |
| isLocal | boolean | Отформатирована ли формула в соответствии с локалью. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Устанавливает значение или выражение, связанное с условным форматированием.

**Remarks**

Пожалуйста, добавьте все области перед установкой формулы. При установке формулы для этого условия, если входное значение начинается с '=', оно будет восприниматься как формула. В противном случае оно будет восприниматься как простое значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\\"=...\\"".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Устанавливает значение или выражение, связанное с этим условием форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Значение или выражение, связанное с этим условием форматирования. Если входное значение начинается с '=', оно будет рассматриваться как формула. В противном случае оно будет рассматриваться как обычное значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\\"=...\\"". |
| isR1C1 | boolean | Является ли формула формулой R1C1. |
| isLocal | boolean | Отформатирована ли формула в соответствии с локалью. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


Устанавливает значение или выражение, связанное с этим условием форматирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula1 | java.lang.String | Значение или выражение, связанное с этим условием форматирования. Если входное значение начинается с '=', оно будет рассматриваться как формула. В противном случае оно будет рассматриваться как обычное значение (текст, число, логическое). Для текстового значения, начинающегося с '=', пользователь может ввести его как формулу в формате: "=\\"=...\\"". |
| formula2 | java.lang.String | Значение или выражение, связанное с этим условием форматирования. Формат ввода такой же, как у formula1. |
| isR1C1 | boolean | Является ли формула формулой R1C1. |
| isLocal | boolean | Отформатирована ли формула в соответствии с локалью. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Устанавливает тип оператора условного формата.

Смотрите [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


Приоритет этого правила условного форматирования. Это значение используется для определения, какое форматирование должно быть оценено и применено. Более низкие числовые значения означают более высокий приоритет по сравнению с более высокими значениями, где '1' — самый высокий приоритет.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


True, правила с более низким приоритетом не могут применяться к этому правилу, когда это правило оценивается как true. Применяется только для Excel 2007;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Получает или задает стиль условно отформатированных диапазонов ячеек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Текстовое значение в правиле условного форматирования "text contains". Действительно только для типов = containsText, notContainsText, beginsWith и endsWith. Значение по умолчанию — null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


Применимый период времени в правиле условного форматирования "date occurrin". Действительно только для типа = timePeriod. Значение по умолчанию — TimePeriodType.Today.

Смотрите [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Устанавливает тип условного формата.

Смотрите [FormatConditionType](../../com.aspose.cells/formatconditiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

