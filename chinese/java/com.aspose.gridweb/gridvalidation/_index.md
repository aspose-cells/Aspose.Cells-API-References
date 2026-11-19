---
title: "GridValidation"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 data validation.settings。"
type: docs
url: /zh/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

表示 data validation.settings。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ServerValidation](#ServerValidation) | 获取或设置服务器端验证 JavaScript 函数名称。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | 在单元格中添加验证设置。 |
| [addACell(String cellname)](#addACell-java.lang.String-) | 在单元格中添加验证设置。 |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | 将验证应用于该区域。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | 表示一个包含数据验证设置的 [GridCellArea](../../com.aspose.gridweb/gridcellarea) 集合。 |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | 获取客户端验证 JavaScript 函数名称。 |
| [getErrorMessage()](#getErrorMessage--) | 表示数据验证错误消息。 |
| [getErrorTitle()](#getErrorTitle--) | 表示数据验证错误对话框的标题。 |
| [getFormula1()](#getFormula1--) | 表示与数据验证关联的值或表达式。 |
| [getFormula2()](#getFormula2--) | 表示与数据验证第二部分关联的值或表达式。 |
| [getInputMessage()](#getInputMessage--) | 表示数据验证错误消息。 |
| [getInputTitle()](#getInputTitle--) | 表示数据验证输入对话框的标题。 |
| [getListValue(int row, int column)](#getListValue-int-int-) | 获取指定单元格的验证列表值。 |
| [getOperator()](#getOperator--) | 表示数据验证的运算符。 |
| [getRegEx()](#getRegEx--) | 获取正则表达式字符串。 |
| [getShowError()](#getShowError--) | 指示当用户输入无效数据时是否显示数据验证错误消息。 |
| [getShowInput()](#getShowInput--) | 指示当用户选择数据验证范围内的单元格时是否显示数据验证输入消息。 |
| [getValidationType()](#getValidationType--) | 获取验证类型。 |
| [getValue1()](#getValue1--) | 表示与数据验证关联的值。 |
| [getValueList()](#getValueList--) | 获取值列表对象。 |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | 获取单元格值是否为必填。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | 删除单元格中的验证设置。 |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | 删除范围内的验证设置。 |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | 设置客户端验证 JavaScript 函数名称。 |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | 表示数据验证错误消息。 |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | 表示数据验证错误对话框的标题。 |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | 表示与数据验证关联的值或表达式。 |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | 表示与数据验证第二部分关联的值或表达式。 |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | 表示数据验证错误消息。 |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | 表示数据验证输入对话框的标题。 |
| [setOperator(int value)](#setOperator-int-) | 表示数据验证的运算符。 |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | 设置正则表达式字符串。 |
| [setRequired(boolean value)](#setRequired-boolean-) | 设置单元格值是否为必填。 |
| [setShowError(boolean value)](#setShowError-boolean-) | 指示当用户输入无效数据时是否显示数据验证错误消息。 |
| [setShowInput(boolean value)](#setShowInput-boolean-) | 指示当用户选择数据验证范围内的单元格时是否显示数据验证输入消息。 |
| [setValidationType(int value)](#setValidationType-int-) | 设置验证类型。 |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | 设置值列表对象。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


获取或设置服务器端验证 JavaScript 函数名称。

**Remarks**

使用 GridCustomServerValidation 属性指定服务器端验证。

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


在单元格中添加验证设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


在单元格中添加验证设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellname | java.lang.String | 单元格名称。 |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


将验证应用于该区域。

**Remarks**

在此方法中，我们将删除此区域的所有旧验证。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 区域。 |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


表示一个包含数据验证设置的 [GridCellArea](../../com.aspose.gridweb/gridcellarea) 集合。

**Remarks**

如果直接将其添加到此列表，区域上的旧验证将不会被删除。

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


获取客户端验证 JavaScript 函数名称。

**Remarks**

使用 ClientValidationFunction 属性指定客户端验证函数的名称。函数应按以下形式声明：
function customValicationFunction(source, value)
参数 "source" 是单元格对象。参数 "value" 是待检查的单元格的字符串值。如果该值有效，函数应返回 true。

**Returns:**
java.lang.String
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
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


表示与数据验证第二部分关联的值或表达式。

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


表示数据验证错误消息。

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
java.lang.Object - 为指定单元格生成此验证列表的值。如果列表引用到一个范围，则返回值将是 ReferredArea 对象；否则返回值可能为 null、object[] 或简单对象。
### getOperator() {#getOperator--}
```
public int getOperator()
```


表示数据验证的运算符。

参见 [GridOperatorType](../../com.aspose.gridweb/gridoperatortype)。

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


获取正则表达式字符串。

**Returns:**
java.lang.String
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
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


获取验证类型。

参见 [GridValidationType](../../com.aspose.gridweb/gridvalidationtype)。

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


表示与数据验证关联的值。

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


获取值列表对象。

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


获取单元格值是否为必填。

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

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


删除范围内的验证设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 包含数据验证设置的范围。 |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


设置客户端验证 JavaScript 函数名称。

**Remarks**

使用 ClientValidationFunction 属性指定客户端验证函数的名称。函数应按以下形式声明：
function customValicationFunction(source, value)
参数 "source" 是单元格对象。参数 "value" 是待检查的单元格的字符串值。如果该值有效，函数应返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


表示与数据验证第二部分关联的值或表达式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


表示数据验证错误消息。

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

参见 [GridOperatorType](../../com.aspose.gridweb/gridoperatortype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


设置正则表达式字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


设置单元格值是否为必填。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


设置验证类型。

参见 [GridValidationType](../../com.aspose.gridweb/gridvalidationtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


设置值列表对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.ArrayList<java.lang.String> |  |

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

