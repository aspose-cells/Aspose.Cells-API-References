---
title: "PivotFieldGroupOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "用于数据透视字段分组设置的选项。"
type: docs
url: /zh/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

用于数据透视字段分组设置的选项。

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
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | 获取离散分组项。 |
| [getEndDate()](#getEndDate--) | 获取分组范围的结束值。 |
| [getEndNumber()](#getEndNumber--) | 获取分组范围的结束值。 |
| [getGroupType()](#getGroupType--) | 获取透视字段的分组类型。 |
| [getGroupTypes()](#getGroupTypes--) | 获取透视字段的分组类型。 |
| [getInterval()](#getInterval--) | 获取每个分组的间隔大小。 |
| [getNewPivotField()](#getNewPivotField--) | 获取一个值，指示分组后是否应创建新的透视字段。 |
| [getStartDate()](#getStartDate--) | 获取分组范围的起始值。 |
| [getStartNumber()](#getStartNumber--) | 获取分组范围的起始值。 |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | 获取一个值，指示结束值是否自动确定。 |
| [isAutoStart()](#isAutoStart--) | 获取一个值，指示起始值是否自动确定。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | 设置一个值，指示结束值是否自动确定。 |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | 设置一个值，指示起始值是否自动确定。 |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | 设置离散分组项。 |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | 设置分组范围的结束值。 |
| [setEndNumber(double value)](#setEndNumber-double-) | 设置分组范围的结束值。 |
| [setGroupType(int value)](#setGroupType-int-) | 设置透视字段的分组类型。 |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | 设置透视字段的分组类型。 |
| [setInterval(double value)](#setInterval-double-) | 设置每个分组的间隔大小。 |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | 设置一个值，指示分组后是否应创建新的透视字段。 |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | 设置分组范围的起始值。 |
| [setStartNumber(double value)](#setStartNumber-double-) | 设置分组范围的起始值。 |
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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


获取离散分组项。

**Remarks**

如果设置了此属性，[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


获取分组范围的结束值。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


获取分组范围的结束值。

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


获取透视字段的分组类型。仅适用于日期时间透视字段的分组。

参见 [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。

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


获取透视字段的分组类型。

参见 [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。

**Remarks**

此属性中的顺序将被忽略。指定多个分组类型时，基础分组字段将按升序插入，而显示分组字段到行/列区域将按降序排列（Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds）。

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


获取每个分组的间隔大小。

**Remarks**

仅适用于数字和天数分组。

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


获取一个值，指示分组后是否应创建新的透视字段。

**Remarks**

如果未显式设置，默认值为数值分组时为 false，日期时间分组时为 true，离散分组时为 true。仅对基础字段的第一个新分组透视字段有效。

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


获取分组范围的起始值。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


获取分组范围的起始值。

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


获取一个值，指示结束值是否自动确定。

**Remarks**

如果设置了 [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) 或 [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--)，此属性将为 false。

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


获取一个值，指示起始值是否自动确定。

**Remarks**

如果设置了 [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) 或 [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--)，此属性将为 false。

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


设置一个值，指示结束值是否自动确定。

**Remarks**

如果设置了 [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) 或 [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--)，此属性将为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


设置一个值，指示起始值是否自动确定。

**Remarks**

如果设置了 [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) 或 [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--)，此属性将为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


设置离散分组项。

**Remarks**

如果设置了此属性，[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


设置分组范围的结束值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


设置分组范围的结束值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


设置透视字段的分组类型。仅适用于日期时间透视字段的分组。

参见 [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


设置透视字段的分组类型。

参见 [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype)。

**Remarks**

此属性中的顺序将被忽略。指定多个分组类型时，基础分组字段将按升序插入，而显示分组字段到行/列区域将按降序排列（Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


设置每个分组的间隔大小。

**Remarks**

仅适用于数字和天数分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


设置一个值，指示分组后是否应创建新的透视字段。

**Remarks**

如果未显式设置，默认值为数值分组时为 false，日期时间分组时为 true，离散分组时为 true。仅对基础字段的第一个新分组透视字段有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


设置分组范围的起始值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


设置分组范围的起始值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

