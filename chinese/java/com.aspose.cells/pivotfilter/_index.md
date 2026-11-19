---
title: "PivotFilter"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 PivotFilter 集合中的一个 PivotFilter。"
type: docs
url: /zh/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

表示 PivotFilter 集合中的一个 PivotFilter。

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
 
         //Add top 10 filter
          pivot.getBaseFields().get(0).filterTop10(0, PivotFilterType.COUNT,false,2);
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | 获取透视过滤器的自动筛选。 |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | 获取数字过滤器的值。 |
| [getEvaluationOrder()](#getEvaluationOrder--) | 获取透视过滤器的评估顺序。 |
| [getFieldIndex()](#getFieldIndex--) | 获取此透视过滤器所应用的源字段索引。 |
| [getFilterCategory()](#getFilterCategory--) | 获取此过滤器的类别。 |
| [getFilterType()](#getFilterType--) | 获取透视过滤器的过滤类型。 |
| [getLabels()](#getLabels--) | 获取标题过滤器的标签。 |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | 指定度量立方体字段的索引。 |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | 获取透视过滤器的度量字段索引。 |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | 获取透视过滤器的成员属性字段索引。 |
| [getName()](#getName--) | 获取透视过滤器的名称。 |
| [getNumberValues()](#getNumberValues--) | 获取数字过滤器的值。 |
| [getTop10Value()](#getTop10Value--) | 获取过滤器的前 10 项设置。 |
| [getUseWholeDay()](#getUseWholeDay--) | 指示是否在日期过滤条件中使用整天。 |
| [getValue1()](#getValue1--) | 获取标签透视过滤器的字符串 value1。 |
| [getValue2()](#getValue2--) | 获取标签透视过滤器的字符串 value2。 |
| [getValueFieldIndex()](#getValueFieldIndex--) | 获取值区域中值字段的索引。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | 获取透视过滤器的评估顺序。 |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | 获取透视过滤器的度量字段索引。 |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | 获取透视过滤器的成员属性字段索引。 |
| [setName(String value)](#setName-java.lang.String-) | 获取透视过滤器的名称。 |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | 指示是否在日期过滤条件中使用整天。 |
| [setValue1(String value)](#setValue1-java.lang.String-) | 获取标签透视过滤器的字符串 value1。 |
| [setValue2(String value)](#setValue2-java.lang.String-) | 获取标签透视过滤器的字符串 value2。 |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | 获取值区域中值字段的索引。 |
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
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


获取透视过滤器的自动筛选。

**Remarks**

注意：此方法现已过时。请改用 FilterLabel、FilterValue、FilterDate 或 FilterTop10 方法。此方法将在自 2024 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDateTimeValues() {#getDateTimeValues--}
```
public DateTime[] getDateTimeValues()
```


获取数字过滤器的值。

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


获取透视过滤器的评估顺序。

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


获取此透视过滤器所应用的源字段索引。

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


获取此过滤器的类别。

参见 [FilterCategory](../../com.aspose.cells/filtercategory)。

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


获取透视过滤器的过滤类型。

请参阅 [PivotFilterType](../../com.aspose.cells/pivotfiltertype)。

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


获取标题过滤器的标签。

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


指定度量立方体字段的索引。此属性仅在 OLAP 数据透视表的过滤器中使用，并指定值过滤器应应用于哪个度量。

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


获取透视过滤器的度量字段索引。

**Remarks**

注意：此方法已过时。请改用 PivotFilter.ValueFieldIndex 属性。该方法将在自 2024 年 11 月起的 12 个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


获取透视过滤器的成员属性字段索引。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取透视过滤器的名称。

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


获取数字过滤器的值。

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


获取过滤器的前 10 项设置。

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


指示是否在日期过滤条件中使用整天。

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


获取标签透视过滤器的字符串 value1。

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


获取标签透视过滤器的字符串 value2。

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


获取值区域中值字段的索引。

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




### setEvaluationOrder(int value) {#setEvaluationOrder-int-}
```
public void setEvaluationOrder(int value)
```


获取透视过滤器的评估顺序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


获取透视过滤器的度量字段索引。

**Remarks**

注意：此方法已过时。请改用 PivotFilter.ValueFieldIndex 属性。该方法将在自 2024 年 11 月起的 12 个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


获取透视过滤器的成员属性字段索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


获取透视过滤器的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


指示是否在日期过滤条件中使用整天。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


获取标签透视过滤器的字符串 value1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


获取标签透视过滤器的字符串 value2。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


获取值区域中值字段的索引。

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

