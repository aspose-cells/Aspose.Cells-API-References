---
title: "Timeline"
second_title: "Aspose.Cells for Java API 参考"
description: "Timeline 视图的概要描述。由于 MS Excel 2003 不支持 Timeline。"
type: docs
url: /zh/java/com.aspose.cells/timeline/
---

**Inheritance:**
java.lang.Object
```
public class Timeline
```

Timeline 视图的摘要说明；由于 Microsoft Excel，Excel 2003 不支持 Timeline。

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
         //Add time line based on date field.
         int index = sheet.getTimelines().add(pivot, "E1","date");
         Timeline timeline = sheet.getTimelines().get(index);
 
         //do your business
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaption()](#getCaption--) | 获取此 Timeline 的标题。 |
| [getClass()](#getClass--) |  |
| [getCurrentLevel()](#getCurrentLevel--) | 时间轴的当前时间级别。 |
| [getHeightPixel()](#getHeightPixel--) | 返回或设置指定时间轴的高度，单位为像素。 |
| [getLeftPixel()](#getLeftPixel--) | 返回或设置时间轴形状相对于左列的水平偏移量，单位为像素。 |
| [getName()](#getName--) | 返回或设置指定时间轴的名称 |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--) | 获取选定的日期时间范围。 |
| [getSelectionLevel()](#getSelectionLevel--) | 获取在时间轴上进行当前选择的时间级别。 |
| [getShape()](#getShape--) | 返回与此时间轴关联的 [TimelineShape](../../com.aspose.cells/timelineshape) 对象。 |
| [getShowHeader()](#getShowHeader--) | 指示是否显示此时间轴的标题。 |
| [getShowHorizontalScrollbar()](#getShowHorizontalScrollbar--) | 指示是否显示水平滚动条。 |
| [getShowSelectionLabel()](#getShowSelectionLabel--) | 指示是否显示选择标签。 |
| [getShowTimeLevel()](#getShowTimeLevel--) | 指示是否显示时间级别的下拉选择框。 |
| [getStartDate()](#getStartDate--) | 获取此 [Timeline](../../com.aspose.cells/timeline) 的时间跨度滚动位置的开始日期。 |
| [getTopPixel()](#getTopPixel--) | 返回或设置时间轴形状相对于顶部行的垂直偏移量，单位为像素。 |
| [getWidthPixel()](#getWidthPixel--) | 返回或设置指定时间轴的宽度，单位为像素。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(DateTime start, DateTime end, boolean calculate)](#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-) | 在日期时间之间选择项目。 |
| [setCaption(String value)](#setCaption-java.lang.String-) | 设置此时间轴的标题。 |
| [setCurrentLevel(int value)](#setCurrentLevel-int-) | 时间轴的当前时间级别。 |
| [setHeightPixel(int value)](#setHeightPixel-int-) | 返回或设置指定时间轴的高度，单位为像素。 |
| [setLeftPixel(int value)](#setLeftPixel-int-) | 返回或设置时间轴形状相对于左列的水平偏移量，单位为像素。 |
| [setName(String value)](#setName-java.lang.String-) | 返回或设置指定时间轴的名称 |
| [setSelectionLevel(int value)](#setSelectionLevel-int-) | 设置在时间轴上进行当前选择的时间级别。 |
| [setShowHeader(boolean value)](#setShowHeader-boolean-) | 指示是否显示此时间轴的标题。 |
| [setShowHorizontalScrollbar(boolean value)](#setShowHorizontalScrollbar-boolean-) | 指示是否显示水平滚动条。 |
| [setShowSelectionLabel(boolean value)](#setShowSelectionLabel-boolean-) | 指示是否显示选择标签。 |
| [setShowTimeLevel(boolean value)](#setShowTimeLevel-boolean-) | 指示是否显示时间级别的下拉选择框。 |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | 设置此 [Timeline](../../com.aspose.cells/timeline) 的时间跨度滚动位置的开始日期。 |
| [setTopPixel(int value)](#setTopPixel-int-) | 返回或设置时间轴形状相对于顶部行的垂直偏移量，单位为像素。 |
| [setWidthPixel(int value)](#setWidthPixel-int-) | 返回或设置指定时间轴的宽度，单位为像素。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


获取此 Timeline 的标题。

**Example**

```
         //Set the caption of this Timeline.
         timeline.setCaption("timeline caption test");
```

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentLevel() {#getCurrentLevel--}
```
public int getCurrentLevel()
```


时间轴的当前时间级别。

参见 [TimelineLevelType](../../com.aspose.cells/timelineleveltype)。

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


返回或设置指定时间轴的高度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Height 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getLeftPixel() {#getLeftPixel--}
```
public int getLeftPixel()
```


返回或设置时间轴形状相对于左列的水平偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Left 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


返回或设置指定时间轴的名称

**Example**

```
         //Set the name of the specified Timeline.
         timeline.setName("timeline name test");
```

**Returns:**
java.lang.String
### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}
```
public DateTime[] getSelectedDateTimeRange()
```


获取选定的日期时间范围。

**Returns:**
com.aspose.cells.DateTime[] -
### getSelectionLevel() {#getSelectionLevel--}
```
public int getSelectionLevel()
```


获取在时间轴上进行当前选择的时间级别。

参见 [TimelineLevelType](../../com.aspose.cells/timelineleveltype)。

**Returns:**
int
### getShape() {#getShape--}
```
public TimelineShape getShape()
```


返回与此时间轴关联的 [TimelineShape](../../com.aspose.cells/timelineshape) 对象。

**Returns:**
[TimelineShape](../../com.aspose.cells/timelineshape)
### getShowHeader() {#getShowHeader--}
```
public boolean getShowHeader()
```


指示是否显示此时间轴的标题。

**Returns:**
boolean
### getShowHorizontalScrollbar() {#getShowHorizontalScrollbar--}
```
public boolean getShowHorizontalScrollbar()
```


指示是否显示水平滚动条。

**Returns:**
boolean
### getShowSelectionLabel() {#getShowSelectionLabel--}
```
public boolean getShowSelectionLabel()
```


指示是否显示选择标签。

**Returns:**
boolean
### getShowTimeLevel() {#getShowTimeLevel--}
```
public boolean getShowTimeLevel()
```


指示是否显示时间级别的下拉选择框。

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


获取此 [Timeline](../../com.aspose.cells/timeline) 的时间跨度滚动位置的开始日期。

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getTopPixel() {#getTopPixel--}
```
public int getTopPixel()
```


返回或设置时间轴形状相对于顶部行的垂直偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Top 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


返回或设置指定时间轴的宽度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Width 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

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




### select(DateTime start, DateTime end, boolean calculate) {#select-com.aspose.cells.DateTime-com.aspose.cells.DateTime-boolean-}
```
public void select(DateTime start, DateTime end, boolean calculate)
```


在日期时间之间选择项目。

**Remarks**

[getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--) must be set before calling this method. If this method is called, [getSelectionLevel()](../../com.aspose.cells/timeline\#getSelectionLevel--) will be [getCurrentLevel()](../../com.aspose.cells/timeline\#getCurrentLevel--).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| start | [DateTime](../../com.aspose.cells/datetime) | 开始日期时间 |
| end | [DateTime](../../com.aspose.cells/datetime) | 结束日期时间 |
| 计算 | boolean | 指示是否计算相对数据透视表 |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


设置此时间轴的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCurrentLevel(int value) {#setCurrentLevel-int-}
```
public void setCurrentLevel(int value)
```


时间轴的当前时间级别。

参见 [TimelineLevelType](../../com.aspose.cells/timelineleveltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


返回或设置指定时间轴的高度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Height 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLeftPixel(int value) {#setLeftPixel-int-}
```
public void setLeftPixel(int value)
```


返回或设置时间轴形状相对于左列的水平偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Left 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


返回或设置指定时间轴的名称

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSelectionLevel(int value) {#setSelectionLevel-int-}
```
public void setSelectionLevel(int value)
```


设置在时间轴上进行当前选择的时间级别。

参见 [TimelineLevelType](../../com.aspose.cells/timelineleveltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowHeader(boolean value) {#setShowHeader-boolean-}
```
public void setShowHeader(boolean value)
```


指示是否显示此时间轴的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowHorizontalScrollbar(boolean value) {#setShowHorizontalScrollbar-boolean-}
```
public void setShowHorizontalScrollbar(boolean value)
```


指示是否显示水平滚动条。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowSelectionLabel(boolean value) {#setShowSelectionLabel-boolean-}
```
public void setShowSelectionLabel(boolean value)
```


指示是否显示选择标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTimeLevel(boolean value) {#setShowTimeLevel-boolean-}
```
public void setShowTimeLevel(boolean value)
```


指示是否显示时间级别的下拉选择框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


设置此 [Timeline](../../com.aspose.cells/timeline) 的时间跨度滚动位置的开始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setTopPixel(int value) {#setTopPixel-int-}
```
public void setTopPixel(int value)
```


返回或设置时间轴形状相对于顶部行的垂直偏移量，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Top 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


返回或设置指定时间轴的宽度，单位为像素。

**Remarks**

注意：此成员已过时。请改用 Shape.Width 属性。该属性将在自2025年5月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

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

