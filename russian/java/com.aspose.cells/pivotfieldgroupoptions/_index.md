---
title: "PivotFieldGroupOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Параметры настройки группировки полей сводной таблицы."
type: docs
url: /ru/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

Параметры настройки группировки полей сводной таблицы.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // Group the first row field (a date field) by months and quarters
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartDate(new DateTime(2008, 1, 1));
         options.setEndDate(new DateTime(2008, 9, 5));
         options.setGroupTypes(new /*PivotGroupByType*/int[] { PivotGroupByType.MONTHS, PivotGroupByType.QUARTERS });
         pt.getRowFields().get(0).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputGroupPivotFieldsInPivotTable.xlsx");
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | Получает дискретные элементы группы. |
| [getEndDate()](#getEndDate--) | Получает конечное значение диапазона группировки. |
| [getEndNumber()](#getEndNumber--) | Получает конечное значение диапазона группировки. |
| [getGroupType()](#getGroupType--) | Получает тип группировки для поля сводной таблицы. |
| [getGroupTypes()](#getGroupTypes--) | Получает тип группировки для поля сводной таблицы. |
| [getInterval()](#getInterval--) | Получает размер интервала для каждой группы. |
| [getNewPivotField()](#getNewPivotField--) | Получает значение, указывающее, следует ли создавать новые поля сводной таблицы после группировки. |
| [getStartDate()](#getStartDate--) | Получает начальное значение диапазона группировки. |
| [getStartNumber()](#getStartNumber--) | Получает начальное значение диапазона группировки. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | Получает значение, указывающее, определяется ли конечное значение автоматически. |
| [isAutoStart()](#isAutoStart--) | Получает значение, указывающее, определяется ли начальное значение автоматически. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | Устанавливает значение, указывающее, определяется ли конечное значение автоматически. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | Устанавливает значение, указывающее, определяется ли начальное значение автоматически. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | Устанавливает дискретные элементы группы. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | Устанавливает конечное значение диапазона группировки. |
| [setEndNumber(double value)](#setEndNumber-double-) | Устанавливает конечное значение диапазона группировки. |
| [setGroupType(int value)](#setGroupType-int-) | Устанавливает тип группировки для поля сводной таблицы. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | Устанавливает тип группировки для поля сводной таблицы. |
| [setInterval(double value)](#setInterval-double-) | Устанавливает размер интервала для каждой группы. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | Устанавливает значение, указывающее, следует ли создавать новые поля сводной таблицы после группировки. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | Устанавливает начальное значение диапазона группировки. |
| [setStartNumber(double value)](#setStartNumber-double-) | Устанавливает начальное значение диапазона группировки. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
```


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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


Получает дискретные элементы группы.

**Remarks**

Если это свойство установлено, [getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


Получает конечное значение диапазона группировки.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


Получает конечное значение диапазона группировки.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


Получает тип группировки для сводного поля. Только для группировки даты и времени сводного поля.

См. [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         //init
         PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
         // Group by year and month together
         /*PivotGroupByType*/int pivotGroupByType = pivotFieldGroupOptions.getGroupType();
         pivotGroupByType = PivotGroupByType.YEARS | PivotGroupByType.MONTHS;
         pivotFieldGroupOptions.setGroupType(pivotGroupByType);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


Получает тип группировки для поля сводной таблицы.

См. [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Порядок в этом свойстве будет игнорироваться. При указании нескольких типов группировки базовые поля группировки будут вставляться в порядке возрастания, а поле группировки будет отображаться в области строк/столбцов в порядке убывания (Годы \\u922b?Кварталы \\u922b?Месяцы \\u922b?Дни \\u922b?Часы \\u922b?Минуты \\u922b?Секунды).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


Получает размер интервала для каждой группы.

**Remarks**

Только для группировки по числам и дням.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


Получает значение, указывающее, следует ли создавать новые поля сводной таблицы после группировки.

**Remarks**

Если не задано явно, значение по умолчанию — false для числовой группировки и true для группировки даты и времени, true для дискретной группы. Работает только для первого нового группирующего сводного поля базового поля.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


Получает начальное значение диапазона группировки.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


Получает начальное значение диапазона группировки.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


Получает значение, указывающее, определяется ли конечное значение автоматически.

**Remarks**

Если [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) или [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) установлены, это свойство будет false.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


Получает значение, указывающее, определяется ли начальное значение автоматически.

**Remarks**

Если [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) или [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) установлены, это свойство будет false.

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




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


Устанавливает значение, указывающее, определяется ли конечное значение автоматически.

**Remarks**

Если [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) или [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--) установлены, это свойство будет false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


Устанавливает значение, указывающее, определяется ли начальное значение автоматически.

**Remarks**

Если [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) или [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--) установлены, это свойство будет false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


Устанавливает дискретные элементы группы.

**Remarks**

Если это свойство установлено, [getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


Устанавливает конечное значение диапазона группировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


Устанавливает конечное значение диапазона группировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


Устанавливает тип группировки для сводного поля. Только для группировки даты и времени сводного поля.

См. [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


Устанавливает тип группировки для поля сводной таблицы.

См. [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

Порядок в этом свойстве будет игнорироваться. При указании нескольких типов группировки базовые поля группировки будут вставляться в порядке возрастания, а поле группировки будет отображаться в области строк/столбцов в порядке убывания (Годы \\u922b?Кварталы \\u922b?Месяцы \\u922b?Дни \\u922b?Часы \\u922b?Минуты \\u922b?Секунды).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


Устанавливает размер интервала для каждой группы.

**Remarks**

Только для группировки по числам и дням.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


Устанавливает значение, указывающее, следует ли создавать новые поля сводной таблицы после группировки.

**Remarks**

Если не задано явно, значение по умолчанию — false для числовой группировки и true для группировки даты и времени, true для дискретной группы. Работает только для первого нового группирующего сводного поля базового поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


Устанавливает начальное значение диапазона группировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


Устанавливает начальное значение диапазона группировки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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

