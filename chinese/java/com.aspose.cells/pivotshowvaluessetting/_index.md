---
title: "PivotShowValuesSetting"
second_title: "Aspose.Cells for Java API 参考"
description: "表示在使用 ShowDataAs 计算时，关于显示值方式的设置。"
type: docs
url: /zh/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

表示在使用 ShowDataAs 计算时，关于显示值方式的设置。

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
## 字段

| 字段 | 描述 |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | 特殊基项索引：使用后续的透视项。 |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | 特殊基项索引：使用前面的透视项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | 表示在使用 ShowDataAs 计算时的基字段。 |
| [getBaseFieldName()](#getBaseFieldName--) | 获取透视基字段的标题。 |
| [getBaseItemCaption()](#getBaseItemCaption--) | 获取基字段中透视项的标题。 |
| [getBaseItemIndex()](#getBaseItemIndex--) | 表示在使用 ShowDataAs 计算时基字段中透视项的自定义索引。 |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | 表示在使用 ShowDataAs 计算时基字段中基透视项的类型。 |
| [getCalculationType()](#getCalculationType--) | 表示在透视报告中如何显示数据字段的值。 |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | 获取在透视报告中如何显示数据字段的值。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | 表示在使用 ShowDataAs 计算时的基字段。 |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | 表示在使用 ShowDataAs 计算时基字段中透视项的自定义索引。 |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | 表示在使用 ShowDataAs 计算时基字段中基透视项的类型。 |
| [setCalculationType(int value)](#setCalculationType-int-) | 表示在透视报告中如何显示数据字段的值。 |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | 设置在透视报告中如何显示数据字段的值。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


特殊基项索引：使用后续的透视项。适用于 "Show Values As" 计算；在 Excel 2010 及更高版本中有效。

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


特殊基项索引：使用前面的透视项。适用于 "Show Values As" 计算；在 Excel 2010 及更高版本中有效。

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


表示在使用 ShowDataAs 计算时的基字段。

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


获取透视基字段的标题。

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


获取基字段中透视项的标题。

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


表示在使用 ShowDataAs 计算时基字段中透视项的自定义索引。

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


表示在使用 ShowDataAs 计算时，基字段中基础透视项的类型。由于 PivotItemPosition.Custom 仅用于读取，如果需要设置 PivotItemPosition.Custom，请设置 PivotField.BaseItemIndex 属性。

请参阅 [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype)。

**Remarks**

注意：此属性现已过时。请改用 PivotShowValuesSetting.BaseItem 属性。此方法将在自 2026 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


表示在透视报告中如何显示数据字段的值。

请参阅 [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat)。

**Remarks**

注意：此属性现已过时。请改用 PivotShowValuesSetting.ShowValuesAs 属性。此方法将在自 2026 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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


获取在透视报告中如何显示数据字段的值。

请参阅 [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype)。

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


表示在使用 ShowDataAs 计算时的基字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


表示在使用 ShowDataAs 计算时基字段中透视项的自定义索引。

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


表示在使用 ShowDataAs 计算时，基字段中基础透视项的类型。由于 PivotItemPosition.Custom 仅用于读取，如果需要设置 PivotItemPosition.Custom，请设置 PivotField.BaseItemIndex 属性。

请参阅 [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype)。

**Remarks**

注意：此属性现已过时。请改用 PivotShowValuesSetting.BaseItem 属性。此方法将在自 2026 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


表示在透视报告中如何显示数据字段的值。

请参阅 [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat)。

**Remarks**

注意：此属性现已过时。请改用 PivotShowValuesSetting.ShowValuesAs 属性。此方法将在自 2026 年 11 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


设置在透视报告中如何显示数据字段的值。

请参阅 [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

