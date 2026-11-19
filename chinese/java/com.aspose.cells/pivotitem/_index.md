---
title: "PivotItem"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据透视字段报告中的一个项。"
type: docs
url: /zh/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

表示数据透视字段报告中的一个项。

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
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## 字段

| 字段 | 描述 |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | 全选哨兵索引（0x7FFD，非有效索引） |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | 获取透视项的日期时间值。如果该值为 null，将返回 DateTime.MinValue |
| [getDoubleValue()](#getDoubleValue--) | 获取透视项的双精度值。如果该值为 null 或非数字，将返回 0 |
| [getFormula()](#getFormula--) | 获取此计算项的公式。 |
| [getIndex()](#getIndex--) | 获取透视项在缓存字段中的索引。 |
| [getName()](#getName--) | 获取透视项的名称。 |
| [getPosition()](#getPosition--) | 指定此项在字段所有 PivotItems 中的索引。 |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | 指定同一父节点下的 PivotItems 中的位置索引。 |
| [getStringValue()](#getStringValue--) | 获取透视项的字符串值。如果该值为 null，将返回 "" |
| [getValue()](#getValue--) | 获取透视项的值 |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | 设置透视项是否隐藏。 |
| [isCalculatedItem()](#isCalculatedItem--) | 指示此透视项是否为计算公式项。 |
| [isDetailHidden()](#isDetailHidden--) | 获取此透视项的详细信息是否隐藏。 |
| [isFormula()](#isFormula--) | 指示此透视项是否为计算公式项。 |
| [isHidden()](#isHidden--) | 获取透视项是否隐藏。 |
| [isHideDetail()](#isHideDetail--) | 获取透视项是否隐藏细节。 |
| [isMissing()](#isMissing--) | 指示该项是否已从数据源中删除。 |
| [move(int offset)](#move-int-) | 在透视字段中上移或下移该项 |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | 上移或下移该项 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | 设置此透视项的细节是否隐藏。 |
| [setFormula(boolean value)](#setFormula-boolean-) | 指示此透视项是否为计算公式项。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 设置透视项是否隐藏。 |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | 设置透视项是否隐藏细节。 |
| [setIndex(int value)](#setIndex-int-) | 获取透视项在缓存字段中的索引。 |
| [setName(String value)](#setName-java.lang.String-) | 获取透视项的名称。 |
| [setPosition(int value)](#setPosition-int-) | 指定此项在字段所有 PivotItems 中的索引。 |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | 指定同一父节点下的 PivotItems 中的位置索引。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


全选哨兵索引（0x7FFD，非有效索引）

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
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


获取透视项的日期时间值。如果该值为 null，将返回 DateTime.MinValue

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


获取透视项的双精度值。如果该值为 null 或非数字，将返回 0

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


获取此计算项的公式。仅在该项为计算项时有效。

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取透视项在缓存字段中的索引。

**Remarks**

注意：此属性已过时。请改用 PivotItem.Position 属性。此方法将在 2026 年 8 月起 6 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取透视项的名称。

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


指定此项在字段所有 PivotItems 中的索引。

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


指定同一父节点下的 PivotItems 中的位置索引。

**Remarks**

注意：此方法已过时。请改用 PivotTable.MoveItem(PivotFieldType, string[],bool,int) 方法。此方法将在 2026 年 11 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


获取透视项的字符串值。如果该值为 null，将返回 ""

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


获取透视项的值

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


设置透视项是否隐藏。

**Remarks**

注意：此成员已过时。请改用 Aspose.Cells.Pivot.PivotItem.IsHidden 属性。此属性将在 2012 年 1 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


指示此透视项是否为计算公式项。

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


获取此透视项的详细信息是否隐藏。

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


指示此透视项是否为计算公式项。

**Remarks**

注意：此属性已过时。请改用 PivotItem.IsCalculatedItem 属性。此属性将在 2024 年 11 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


获取透视项是否隐藏。

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


获取透视项是否隐藏细节。

**Remarks**

注意：此属性已过时。请改用 PivotItem.IsDetailHidden 属性。此属性将在 2024 年 11 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


指示该项是否已从数据源中删除。

**Remarks**

True 表示该值已从数据源中删除。

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


在透视字段中上移或下移该项

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 偏移 | int | 上移或下移的次数。如果小于零则上移该项；如果大于零则下移该项。 |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


上移或下移该项

**Remarks**

注意：此方法已过时。请改用 PivotTable.MoveItem(PivotFieldType, string[],bool,int) 或 PivotItem.Move(int) 方法。此方法将在 2026 年 11 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 偏移 | int | 上移或下移的次数。如果小于零则上移该项；如果大于零则下移该项。 |
| isSameParent | boolean | 指定移动操作是否在同一父节点中 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


设置此透视项的细节是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


指示此透视项是否为计算公式项。

**Remarks**

注意：此属性已过时。请改用 PivotItem.IsCalculatedItem 属性。此属性将在 2024 年 11 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


设置透视项是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


设置透视项是否隐藏细节。

**Remarks**

注意：此属性已过时。请改用 PivotItem.IsDetailHidden 属性。此属性将在 2024 年 11 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


获取透视项在缓存字段中的索引。

**Remarks**

注意：此属性已过时。请改用 PivotItem.Position 属性。此方法将在 2026 年 8 月起 6 个月后移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


获取透视项的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


指定此项在字段所有 PivotItems 中的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


指定同一父节点下的 PivotItems 中的位置索引。

**Remarks**

注意：此方法已过时。请改用 PivotTable.MoveItem(PivotFieldType, string[],bool,int) 方法。此方法将在 2026 年 11 月起 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

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

