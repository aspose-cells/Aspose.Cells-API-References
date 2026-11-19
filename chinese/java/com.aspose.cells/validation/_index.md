---
title: "验证"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 data validation.settings。"
type: docs
url: /zh/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

表示 data validation.settings。

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | 将验证应用于该区域。 |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | 将验证应用于该区域。 |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | 将验证应用于给定的区域。 |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | 复制验证。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | 表示验证警报样式。 |
| [getAreas()](#getAreas--) | 获取所有包含数据验证设置的 [CellArea](../../com.aspose.cells/cellarea)。 |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | 表示数据验证错误消息。 |
| [getErrorTitle()](#getErrorTitle--) | 表示数据验证错误对话框的标题。 |
| [getFormula1()](#getFormula1--) | 表示与数据验证关联的值或表达式。 |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | 获取与此验证关联的值或表达式。 |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | 获取特定单元格的此验证关联的值或表达式。 |
| [getFormula2()](#getFormula2--) | 表示与数据验证关联的值或表达式。 |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | 获取与此验证关联的值或表达式。 |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | 获取特定单元格的此验证关联的值或表达式。 |
| [getIgnoreBlank()](#getIgnoreBlank--) | 指示范围数据验证是否允许空值。 |
| [getInCellDropDown()](#getInCellDropDown--) | 指示数据验证是否显示包含可接受值的下拉列表。 |
| [getInputMessage()](#getInputMessage--) | 表示数据验证输入消息。 |
| [getInputTitle()](#getInputTitle--) | 表示数据验证输入对话框的标题。 |
| [getListValue(int row, int column)](#getListValue-int-int-) | 获取指定单元格的验证列表值。 |
| [getOperator()](#getOperator--) | 表示数据验证的运算符。 |
| [getShowError()](#getShowError--) | 指示当用户输入无效数据时是否显示数据验证错误消息。 |
| [getShowInput()](#getShowInput--) | 指示当用户选择数据验证范围内的单元格时是否显示数据验证输入消息。 |
| [getType()](#getType--) | 表示数据验证类型。 |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | 获取特定单元格上验证的值。 |
| [getValue1()](#getValue1--) | 表示与数据验证关联的第一个值。 |
| [getValue2()](#getValue2--) | 表示与数据验证关联的第二个值。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | 删除单元格中的验证设置。 |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | 删除范围内的验证设置。 |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | 从给定区域中移除此验证。 |
| [setAlertStyle(int value)](#setAlertStyle-int-) | 表示验证警报样式。 |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | 表示数据验证错误消息。 |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | 表示数据验证错误对话框的标题。 |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | 表示与数据验证关联的值或表达式。 |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | 设置与此验证关联的值或表达式。 |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | 表示与数据验证关联的值或表达式。 |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | 设置与此验证关联的值或表达式。 |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | 指示范围数据验证是否允许空值。 |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | 指示数据验证是否显示包含可接受值的下拉列表。 |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | 表示数据验证输入消息。 |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | 表示数据验证输入对话框的标题。 |
| [setOperator(int value)](#setOperator-int-) | 表示数据验证的运算符。 |
| [setShowError(boolean value)](#setShowError-boolean-) | 指示当用户输入无效数据时是否显示数据验证错误消息。 |
| [setShowInput(boolean value)](#setShowInput-boolean-) | 指示当用户选择数据验证范围内的单元格时是否显示数据验证输入消息。 |
| [setType(int value)](#setType-int-) | 表示数据验证类型。 |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | 表示与数据验证关联的第一个值。 |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | 表示与数据验证关联的第二个值。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


将验证应用于该区域。

**Remarks**

等同于使用 [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) 并检查交叉和边缘。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | 区域。 |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


将验证应用于该区域。

**Remarks**

在此方法中，我们将删除给定区域中的所有旧验证。对于 Validation 应用范围的左上角区域，首先其 StartRow 最小，其次在具有相同最小 StartRow 的区域中，其 StartColumn 最小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | 区域。 |
| checkIntersection | boolean | 是否检查给定区域与已有验证区域的交叉。如果已有验证已应用于给定区域（或其部分），则应首先从该区域移除已有验证。否则可能导致生成的验证损坏。如果用户确信添加的区域不会与任何已有区域相交，则可将此参数设为 false，以提升性能。 |
| checkEdge | boolean | 是否检查此验证应用区域的边缘。Validation 的内部设置依赖于其应用范围的左上角区域，如果给定区域将成为新的左上角区域，则需要更改并重新构建内部设置，否则可能导致意外结果。如果用户确信添加的区域不是左上角区域，可将此参数设为 false，以提升性能。 |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


将验证应用于给定的区域。

**Remarks**

在此方法中，我们将删除给定区域中的所有旧验证。对于 Validation 应用范围的左上角区域，首先其 StartRow 最小，其次在具有相同最小 StartRow 的区域中，其 StartColumn 最小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | 这些区域。 |
| checkIntersection | boolean | 是否检查给定区域与已有验证区域的交叉。如果已有验证已应用于给定区域（或其部分），则应首先从该区域移除已有验证。否则可能导致生成的验证损坏。如果用户确信所有添加的区域都不与任何已有区域相交，则可将此参数设为 false，以提升性能。 |
| checkEdge | boolean | 是否检查此验证应用区域的边缘。Validation 的内部设置依赖于其应用范围的左上角区域，如果给定的某个区域将成为新的左上角区域，则需要更改并重新构建内部设置，否则可能导致意外结果。如果用户确信这些添加的区域中没有任何一个是左上角区域，可将此参数设为 false，以提升性能。 |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


复制验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | 源验证。 |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | 复制选项。 |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


表示验证警报样式。

参见 [ValidationAlertType](../../com.aspose.cells/validationalerttype)。

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


获取所有包含数据验证设置的 [CellArea](../../com.aspose.cells/cellarea)。

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


表示数据验证错误消息。

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


表示数据验证错误对话框的标题。

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


表示与数据验证关联的值或表达式。

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


获取与此验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 与此验证关联的值或表达式。
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


获取特定单元格的此验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 与此验证关联的值或表达式。
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


表示与数据验证关联的值或表达式。

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


获取与此验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |

**Returns:**
java.lang.String - 与此验证关联的值或表达式。
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


获取特定单元格的此验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isR1C1 | boolean | 公式是否需要以 R1C1 格式化。 |
| isLocal | boolean | 公式是否需要根据区域设置进行格式化。 |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 与此验证关联的值或表达式。
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


指示范围数据验证是否允许空值。

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


指示数据验证是否显示包含可接受值的下拉列表。

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


表示数据验证输入消息。

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


表示数据验证输入对话框的标题。

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


获取指定单元格的验证列表值。

**Remarks**

仅适用于类型为 List 且已应用于给定单元格的验证，否则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.Object - 为指定单元格生成此验证的列表的值。如果列表引用了一个范围，则返回值将是一个 [ReferredArea](../../com.aspose.cells/referredarea) 对象；否则返回值可能为 null、object[] 或简单对象。
### getOperator() {#getOperator--}
```
public int getOperator()
```


表示数据验证的运算符。

请参阅 [OperatorType](../../com.aspose.cells/operatortype)。

**Returns:**
int
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


指示当用户输入无效数据时是否显示数据验证错误消息。

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


指示当用户选择数据验证范围内的单元格时是否显示数据验证输入消息。

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


表示数据验证类型。

请参阅 [ValidationType](../../com.aspose.cells/validationtype)。

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


获取特定单元格上验证的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |
| isValue1 | boolean | 指示是否获取第一个值。 |

**Returns:**
java.lang.Object - 
### getValue1() {#getValue1--}
```
public Object getValue1()
```


表示与数据验证关联的第一个值。

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


表示与数据验证关联的第二个值。

**Returns:**
java.lang.Object
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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


删除单元格中的验证设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


删除范围内的验证设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | 应删除此验证设置的区域。 |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


从给定区域中移除此验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | 应删除此验证设置的区域。 |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


表示验证警报样式。

参见 [ValidationAlertType](../../com.aspose.cells/validationalerttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


表示数据验证错误消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


表示数据验证错误对话框的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


表示与数据验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


设置与此验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 与此格式条件关联的值或表达式。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式。 |
| isLocal | boolean | 公式是否已本地化格式化。 |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


表示与数据验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


设置与此验证关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 与此格式条件关联的值或表达式。 |
| isR1C1 | boolean | 公式是否为 R1C1 公式。 |
| isLocal | boolean | 公式是否已本地化格式化。 |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


指示范围数据验证是否允许空值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


指示数据验证是否显示包含可接受值的下拉列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


表示数据验证输入消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


表示数据验证输入对话框的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


表示数据验证的运算符。

请参阅 [OperatorType](../../com.aspose.cells/operatortype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


指示当用户输入无效数据时是否显示数据验证错误消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


指示当用户选择数据验证范围内的单元格时是否显示数据验证输入消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


表示数据验证类型。

请参阅 [ValidationType](../../com.aspose.cells/validationtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


表示与数据验证关联的第一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


表示与数据验证关联的第二个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

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

