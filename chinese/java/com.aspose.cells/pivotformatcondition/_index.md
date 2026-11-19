---
title: "PivotFormatCondition"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 PivotFormatCondition 集合中的一个数据透视表格式条件。"
type: docs
url: /zh/java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

表示 PivotFormatCondition 集合中的一个数据透视表格式条件。

**Remarks**

注意：此类已过时。请改用 [PivotConditionalFormat](../../com.aspose.cells/pivotconditionalformat) 类。此方法将在自 2024 年 12 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Example**

```
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | 在列字段中添加 PivotTable 条件格式限制。 |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | 在列字段中添加 PivotTable 条件格式限制。 |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | 在数据字段中添加 PivotTable 条件格式限制。 |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | 在数据字段中添加 PivotTable 条件格式限制。 |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | 在行字段中添加 PivotTable 条件格式限制。 |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | 在行字段中添加 PivotTable 条件格式限制。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | 获取数据透视表条件格式的条件。 |
| [getRuleType()](#getRuleType--) | 获取数据透视表条件格式的规则类型。 |
| [getScopeType()](#getScopeType--) | 获取数据透视表条件格式的作用域类型。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | 设置 PivotFormatCondition 对象的条件区域。 |
| [setRuleType(int value)](#setRuleType-int-) | 设置数据透视表条件格式的规则类型。 |
| [setScopeType(int value)](#setScopeType-int-) | 设置数据透视表条件格式的作用域类型。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


在列字段中添加 PivotTable 条件格式限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | 列字段中的 PivotField。 |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


在列字段中添加 PivotTable 条件格式限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField 的名称。 |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


在数据字段中添加 PivotTable 条件格式限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | 数据字段中的 PivotField。 |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


在数据字段中添加 PivotTable 条件格式限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField 的名称。 |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


在行字段中添加 PivotTable 条件格式限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | 行字段中的 PivotField。 |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


在行字段中添加 PivotTable 条件格式限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldName | java.lang.String | PivotField 的名称。 |

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
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


获取数据透视表条件格式的条件。

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


获取数据透视表条件格式的规则类型。

参见 [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


获取数据透视表条件格式的作用域类型。

参见 [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


设置 PivotFormatCondition 对象的条件区域。

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


设置数据透视表条件格式的规则类型。

参见 [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


设置数据透视表条件格式的作用域类型。

参见 [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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

