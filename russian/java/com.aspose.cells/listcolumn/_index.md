---
title: "ListColumn"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет столбец в таблице."
type: docs
url: /ru/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

Представляет столбец в таблице.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Получает формулу этого столбца списка. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Получает формулу строки итогов этого столбца списка. |
| [getDataStyle()](#getDataStyle--) | Получает стиль данных в этом столбце таблицы. |
| [getFormula()](#getFormula--) | Получает формулу столбца списка. |
| [getName()](#getName--) | Получает имя столбца. |
| [getRange()](#getRange--) | Получает диапазон этого столбца списка. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Получает тип вычисления в строке Итого столбца списка. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Получает отображаемые метки строки Итого. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Указывает, является ли формула массивной формулой. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Устанавливает формулу для этого столбца списка. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Получает формулу строки итогов этого столбца списка. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Устанавливает стиль данных в этом столбце таблицы. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Устанавливает формулу столбца списка. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя столбца. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Устанавливает тип вычисления в строке Итого столбца списка. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Устанавливает отображаемые метки строки Итого. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


Получает формулу этого столбца списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String - Формула этого столбца списка.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


Получает формулу строки итогов этого столбца списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String - Формула этого столбца списка.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


Получает стиль данных в этом столбце таблицы.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Получает формулу столбца списка.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Получает имя столбца.

**Remarks**

Если установить имя столбца, соответствующее значение ячейки также будет изменено.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


Получает диапазон этого столбца списка.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


Получает тип вычисления в строке Итого столбца списка.

См. [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


Получает отображаемые метки строки Итого.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Указывает, является ли формула массивной формулой.

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




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


Устанавливает формулу для этого столбца списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | формула для этого столбца списка. |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


Получает формулу строки итогов этого столбца списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | формула для этого столбца списка. |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


Устанавливает стиль данных в этом столбце таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Устанавливает формулу столбца списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя столбца.

**Remarks**

Если установить имя столбца, соответствующее значение ячейки также будет изменено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


Устанавливает тип вычисления в строке Итого столбца списка.

См. [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


Устанавливает отображаемые метки строки Итого.

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

