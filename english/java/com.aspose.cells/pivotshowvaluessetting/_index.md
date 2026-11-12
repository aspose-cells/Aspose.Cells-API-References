---
title: PivotShowValuesSetting
second_title: Aspose.Cells for Java API Reference
description: Represents the settings about showing values as when the ShowDataAs calculation is in use.
type: docs
url: /java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

Represents the settings about showing values as when the ShowDataAs calculation is in use.

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
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Fields

| Field | Description |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Special base item index: use the succeeding pivot item. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Special base item index: use the preceding pivot item. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [getBaseFieldName()](#getBaseFieldName--) | Gets caption of the pivot base field. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Gets caption of the pivot item in the base field. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. |
| [getCalculationType()](#getCalculationType--) | Represents how to show values of a data field in the pivot report. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Gets how to show values of a data field in the pivot report. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. |
| [setCalculationType(int value)](#setCalculationType-int-) | Represents how to show values of a data field in the pivot report. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Sets how to show values of a data field in the pivot report. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Special base item index: use the succeeding pivot item. Valid for "Show Values As" calculations; effective in Excel 2010 and later.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Special base item index: use the preceding pivot item. Valid for "Show Values As" calculations; effective in Excel 2010 and later.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Gets caption of the pivot base field.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Gets caption of the pivot item in the base field.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

See [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.BaseItem property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Represents how to show values of a data field in the pivot report.

See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.ShowValuesAs property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


Gets how to show values of a data field in the pivot report.

See [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

See [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.BaseItem property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Represents how to show values of a data field in the pivot report.

See [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotShowValuesSetting.ShowValuesAs property instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Sets how to show values of a data field in the pivot report.

See [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

