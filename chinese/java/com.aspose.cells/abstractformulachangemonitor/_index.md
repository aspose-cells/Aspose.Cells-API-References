---
title: "AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells for Java API 参考"
description: "为用户提供监视，以跟踪特定操作期间公式的更改。"
type: docs
url: /zh/java/com.aspose.cells/abstractformulachangemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractFormulaChangeMonitor
```

为用户提供监视，以跟踪特定操作期间公式的更改。

**Remarks**

例如，在删除/插入单元格范围时，其他单元格的公式可能会因引用的移动而发生更改。请注意，监视器中的方法可能会针对包含该公式的同一对象被调用多次。

**Example**

```
         class MyFormulaChangeMonitor extends AbstractFormulaChangeMonitor
         {
             private final WorksheetCollection mWorksheets;
             public MyFormulaChangeMonitor(WorksheetCollection worksheets)
             {
                 mWorksheets = worksheets;
             }
             public /*override*/ void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
             {
                 System.out.println("Cell " + mWorksheets.get(sheetIndex).getName() + "!"
                     + CellsHelper.cellIndexToName(rowIndex, columnIndex)
                     + "'s formula was changed while inserting rows.");
             }
         }
         Workbook wb = new Workbook("template.xlsx");
         InsertOptions options = new InsertOptions();
         options.setFormulaChangeMonitor(new MyFormulaChangeMonitor(wb.getWorksheets()));
         wb.getWorksheets().get(0).getCells().insertRows(0, 2, options);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractFormulaChangeMonitor()](#AbstractFormulaChangeMonitor--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)](#onCellFormulaChanged-int-int-int-) | 当单元格中的公式被更改时将触发的事件。 |
| [onFormatConditionFormulaChanged(FormatCondition fc)](#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-) | 当 FormatCondition 的公式被更改时将触发的事件。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractFormulaChangeMonitor() {#AbstractFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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




### onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex) {#onCellFormulaChanged-int-int-int-}
```
public void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```


当单元格中的公式被更改时将触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 已更改单元格的工作表索引 |
| rowIndex | int | 已更改单元格的行索引 |
| columnIndex | int | 已更改单元格的列索引 |

### onFormatConditionFormulaChanged(FormatCondition fc) {#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-}
```
public void onFormatConditionFormulaChanged(FormatCondition fc)
```


当 FormatCondition 的公式被更改时将触发的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fc | [FormatCondition](../../com.aspose.cells/formatcondition) | 公式已更改的 FormatCondition 对象 |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

