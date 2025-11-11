---
title: TableStyle
second_title: Aspose.Cells for Java API Reference
description: Represents the style of the table.
type: docs
url: /java/com.aspose.cells/tablestyle/
---

**Inheritance:**
java.lang.Object
```
public class TableStyle
```

Represents the style of the table.

**Example**

```
         Workbook workbook = new Workbook();
         Style firstColumnStyle = workbook.createStyle();
         firstColumnStyle.setPattern(BackgroundType.SOLID);
         firstColumnStyle.setBackgroundColor(com.aspose.cells.Color.getRed());
 
         Style lastColumnStyle = workbook.createStyle();
         lastColumnStyle.getFont().setBold(true);
         lastColumnStyle.setPattern(BackgroundType.SOLID);
         lastColumnStyle.setBackgroundColor(com.aspose.cells.Color.getRed());
         String tableStyleName = "Custom1";
         TableStyleCollection tableStyles = workbook.getWorksheets().getTableStyles();
         int index1 = tableStyles.addTableStyle(tableStyleName);
         TableStyle tableStyle = tableStyles.get(index1);
         TableStyleElementCollection elements = tableStyle.getTableStyleElements();
         index1 = elements.add(TableStyleElementType.FIRST_COLUMN);
         TableStyleElement element = elements.get(index1);
         element.setElementStyle(firstColumnStyle);
         index1 = elements.add(TableStyleElementType.LAST_COLUMN);
         element = elements.get(index1);
         element.setElementStyle(lastColumnStyle);
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
             cells.get(0, i).putValue(CellsHelper.columnIndexToName(i));
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
         table.setShowTableStyleFirstColumn(true);
         table.setShowTableStyleLastColumn(true);
         table.setTableStyleName(tableStyleName);
         workbook.save("Book1.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Gets the name of table style. |
| [getTableStyleElements()](#getTableStyleElements--) | Gets all elements of the table style. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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
### getName() {#getName--}
```
public String getName()
```


Gets the name of table style.

**Returns:**
java.lang.String
### getTableStyleElements() {#getTableStyleElements--}
```
public TableStyleElementCollection getTableStyleElements()
```


Gets all elements of the table style.

**Returns:**
[TableStyleElementCollection](../../com.aspose.cells/tablestyleelementcollection)
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

