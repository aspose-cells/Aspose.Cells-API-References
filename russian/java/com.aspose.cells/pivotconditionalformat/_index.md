---
title: "PivotConditionalFormat"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет условный формат сводной таблицы."
type: docs
url: /ru/java/com.aspose.cells/pivotconditionalformat/
---

**Inheritance:**
java.lang.Object
```
public class PivotConditionalFormat
```

Представляет условный формат сводной таблицы.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
 
 
         //do your business
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addCellArea(CellArea ca)](#addCellArea-com.aspose.cells.CellArea-) | Добавляет область на основе представления сводной таблицы. |
| [addFieldArea(int axisType, PivotField field)](#addFieldArea-int-com.aspose.cells.PivotField-) | Добавляет область поля сводной таблицы. |
| [addFieldArea(int axisType, String fieldName)](#addFieldArea-int-java.lang.String-) | Добавляет область поля сводной таблицы. |
| [applyTo(int row, int column, int scope)](#applyTo-int-int-int-) | Применяет условное форматирование к диапазону, который должен находиться в области данных. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellAreas()](#getCellAreas--) | Получает все ячейковые области, к которым применяется это условное форматирование. |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Получить условия для условного форматирования сводной таблицы. |
| [getPivotAreas()](#getPivotAreas--) | Получает все области сводной таблицы. |
| [getRuleType()](#getRuleType--) | Получает тип правила для условного форматирования сводной таблицы. |
| [getScopeType()](#getScopeType--) | Получает тип области для условного форматирования сводной таблицы. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRuleType(int value)](#setRuleType-int-) | Устанавливает тип правила для условного форматирования сводной таблицы. |
| [setScopeType(int value)](#setScopeType-int-) | Устанавливает тип области для условного форматирования сводной таблицы. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCellArea(CellArea ca) {#addCellArea-com.aspose.cells.CellArea-}
```
public void addCellArea(CellArea ca)
```


Добавляет область на основе представления сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Область ячейки. |

### addFieldArea(int axisType, PivotField field) {#addFieldArea-int-com.aspose.cells.PivotField-}
```
public void addFieldArea(int axisType, PivotField field)
```


Добавляет область поля сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Поле сводной таблицы. |

### addFieldArea(int axisType, String fieldName) {#addFieldArea-int-java.lang.String-}
```
public void addFieldArea(int axisType, String fieldName)
```


Добавляет область поля сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Тип области. |
| fieldName | java.lang.String | Имя поля сводной таблицы. |

### applyTo(int row, int column, int scope) {#applyTo-int-int-int-}
```
public void applyTo(int row, int column, int scope)
```


Применяет условное форматирование к диапазону, который должен находиться в области данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | int | Выбранная строка. |
| столбец | int | Выбранный столбец. |
| scope | int | [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype). Область |

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
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Получает все ячейковые области, к которым применяется это условное форматирование.

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Получить условия для условного форматирования сводной таблицы.

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getPivotAreas() {#getPivotAreas--}
```
public PivotAreaCollection getPivotAreas()
```


Получает все области сводной таблицы.

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Получает тип правила для условного форматирования сводной таблицы.

См. [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Получает тип области для условного форматирования сводной таблицы.

См. [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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




### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Устанавливает тип правила для условного форматирования сводной таблицы.

См. [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Устанавливает тип области для условного форматирования сводной таблицы.

См. [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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

