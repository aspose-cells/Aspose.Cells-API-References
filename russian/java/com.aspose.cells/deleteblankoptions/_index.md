---
title: "DeleteBlankOptions"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройку удаления пустых ячеек/строк/столбцов."
type: docs
url: /ru/java/com.aspose.cells/deleteblankoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```

Представляет настройку удаления пустых ячеек/строк/столбцов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Указывает, будут ли объекты, связанные с рисованием, такие как изображение, фигура, диаграмма..., считаться пустыми. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Будет ли одна ячейка считаться пустой, если она содержит формулу, а вычисленный результат равен null или пустой строке. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Указывает, будет ли одна ячейка считаться пустой, когда её значение — пустая строка. |
| [getEndIndex()](#getEndIndex--) | Задает конечный индекс строки/столбца (включительно) диапазона, в котором проверяются и удаляются пустые строки/столбцы. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Получает монитор для отслеживания изменений, вызванных удалением. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов. |
| [getStartIndex()](#getStartIndex--) | Задает начальный индекс строки/столбца диапазона, в котором проверяются и удаляются пустые строки/столбцы. |
| [getUpdateReference()](#getUpdateReference--) | Указывает, следует ли обновлять ссылки в других листах. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Указывает, будут ли объекты, связанные с рисованием, такие как изображение, фигура, диаграмма..., считаться пустыми. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Будет ли одна ячейка считаться пустой, если она содержит формулу, а вычисленный результат равен null или пустой строке. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Указывает, будет ли одна ячейка считаться пустой, когда её значение — пустая строка. |
| [setEndIndex(int value)](#setEndIndex-int-) | Задает конечный индекс строки/столбца (включительно) диапазона, в котором проверяются и удаляются пустые строки/столбцы. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Устанавливает монитор для отслеживания изменений, вызванных удалением. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов. |
| [setStartIndex(int value)](#setStartIndex-int-) | Задает начальный индекс строки/столбца диапазона, в котором проверяются и удаляются пустые строки/столбцы. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Указывает, следует ли обновлять ссылки в других листах. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```


Указывает, будут ли объекты, связанные с рисованием, такие как изображение, фигура, диаграмма..., считаться пустыми. Значение по умолчанию — true.

**Remarks**

При установке этого свойства в false все строки/столбцы, покрытые объектами рисования, не будут считаться пустыми и не будут удалены.

**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```


Будет ли ячейка считаться пустой, если она содержит формулу, а вычисленный результат равен null или пустой строке. Значение по умолчанию — false.

**Remarks**

Как правило, пользователь должен убедиться, что формулы вычислены до операции удаления, когда это свойство установлено в true. В противном случае все недавно созданные формулы обычными API, такими как [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--), будут считаться пустыми и могут быть удалены, поскольку до вычисления их результаты равны null.

**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```


Указывает, будет ли ячейка считаться пустой, когда её значение — пустая строка. Значение по умолчанию — true.

**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```


Задает конечный индекс строки/столбца (включительно) диапазона для проверки и удаления пустых строк/столбцов. Значение по умолчанию — -1, а -1 означает максимальный диапазон всех объектов (ячеек, рисунков и т.д.), которые необходимо проверять.

**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```


Получает монитор для отслеживания изменений, вызванных удалением.

**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```


Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов.

Смотрите [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Для [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) все ячейки в диапазоне считаются пустыми, за исключением непустой верхней левой ячейки. Это значение по умолчанию для данного свойства.

Для [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) все ячейки в диапазоне считаются непустыми.

Для [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) все ячейки за пределами области отображения содержимого считаются пустыми.



**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Задает начальный индекс строки/столбца диапазона, в котором проверяются и удаляются пустые строки/столбцы.

**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Указывает, следует ли обновлять ссылки в других листах.

**Remarks**

Начиная с версии 26.7, мы установили значение по умолчанию этого свойства в true.

**Returns:**
boolean
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




### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```


Указывает, будут ли объекты, связанные с рисованием, такие как изображение, фигура, диаграмма..., считаться пустыми. Значение по умолчанию — true.

**Remarks**

При установке этого свойства в false все строки/столбцы, покрытые объектами рисования, не будут считаться пустыми и не будут удалены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```


Будет ли ячейка считаться пустой, если она содержит формулу, а вычисленный результат равен null или пустой строке. Значение по умолчанию — false.

**Remarks**

Как правило, пользователь должен убедиться, что формулы вычислены до операции удаления, когда это свойство установлено в true. В противном случае все недавно созданные формулы обычными API, такими как [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--), будут считаться пустыми и могут быть удалены, поскольку до вычисления их результаты равны null.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```


Указывает, будет ли ячейка считаться пустой, когда её значение — пустая строка. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```


Задает конечный индекс строки/столбца (включительно) диапазона для проверки и удаления пустых строк/столбцов. Значение по умолчанию — -1, а -1 означает максимальный диапазон всех объектов (ячеек, рисунков и т.д.), которые необходимо проверять.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```


Устанавливает монитор для отслеживания изменений, вызванных удалением.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |

### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```


Указывает, как обрабатывать объединённые ячейки при удалении пустых строк/столбцов.

Смотрите [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).

**Remarks**

Для [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY) все ячейки в диапазоне считаются пустыми, за исключением непустой верхней левой ячейки. Это значение по умолчанию для данного свойства.

Для [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE) все ячейки в диапазоне считаются непустыми.

Для [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT) все ячейки за пределами области отображения содержимого считаются пустыми.



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```


Задает начальный индекс строки/столбца диапазона, в котором проверяются и удаляются пустые строки/столбцы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Указывает, следует ли обновлять ссылки в других листах.

**Remarks**

Начиная с версии 26.7, мы установили значение по умолчанию этого свойства в true.

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

