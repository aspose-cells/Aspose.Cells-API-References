---
title: "GridCell"
second_title: "Aspose.Cells for Java API 参考"
description: "表示单元格对象。"
type: docs
url: /zh/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

表示单元格对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | 指示此单元格是否包含外部链接。 |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | 从源单元格复制数据。 |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | 复制样式并为单元格设置样式。 |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | 为单元格创建评论对象。 |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | 为单元格创建验证对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 检查此对象是否与另一个单元格对象引用相同的单元格。 |
| [getBoolValue()](#getBoolValue--) | 获取单元格中包含的布尔值。 |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | 获取单元格的列号（从零开始）。 |
| [getComment()](#getComment--) | 获取此单元格上的评论对象。 |
| [getDateValue()](#getDateValue--) | 获取单元格中包含的 DateTime 值。 |
| [getDisplayStringValue()](#getDisplayStringValue--) | 获取此单元格的格式化字符串值。 |
| [getDoubleValue()](#getDoubleValue--) | 获取单元格中包含的 double 值。 |
| [getFloatValue()](#getFloatValue--) | 获取单元格中包含的 float 值。 |
| [getFormula()](#getFormula--) | 获取 [GridCell](../../com.aspose.gridweb/gridcell) 的公式。 |
| [getHtmlString()](#getHtmlString--) | 获取包含此单元格数据和部分格式的 HTML 字符串。 |
| [getIntValue()](#getIntValue--) | 获取单元格中包含的整数值。 |
| [getName()](#getName--) | 获取单元格的名称。 |
| [getRow()](#getRow--) | 获取单元格的行号（从零开始）。 |
| [getStringValue()](#getStringValue--) | 获取单元格中包含的字符串值。 |
| [getStyle()](#getStyle--) | 获取单元格样式的副本。为单元格设置样式。 |
| [getType()](#getType--) | 返回单元格值类型，含义请参见 GridCellValueType.java。 |
| [getValue()](#getValue--) | 获取此单元格中包含的值。 |
| [getWidthOfValue()](#getWidthOfValue--) | 获取该值的宽度，单位为像素。 |
| [hashCode()](#hashCode--) | 作为特定类型的哈希函数。 |
| [isErrorValue()](#isErrorValue--) | 检查公式是否能够正确计算结果。 |
| [isFormula()](#isFormula--) | 表示指定的单元格是否包含公式。 |
| [isStyleSet()](#isStyleSet--) | 指示是否已设置单元格的样式。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | 将布尔值写入单元格。 |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | 将 DateTime 值写入单元格。 |
| [putValue(double param_double)](#putValue-double-) | 将 double 值写入单元格。 |
| [putValue(int param_int)](#putValue-int-) | 将一个 int 值放入单元格。 |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | 将对象值放入单元格。相当于 setValue(Object param\_object)。 |
| [putValue(String param_string)](#putValue-java.lang.String-) | 将一个 String 值放入单元格。 |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | 将字符串值写入单元格，并在适当时将其转换为其他数据类型。 |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | 将值写入单元格，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | 使用字符串值设置单元格的值，并根据该值设置单元格格式。 |
| [removeComment()](#removeComment--) | 移除单元格的注释对象。 |
| [removeValidation()](#removeValidation--) | 移除单元格的验证对象。 |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | 为单元格设置边框（上、下、左、右），所有边框使用相同的边框样式。 |
| [setCustom(String custom)](#setCustom-java.lang.String-) | 设置自定义格式，null 或空字符串表示没有自定义格式。 |
| [setFormula(String value)](#setFormula-java.lang.String-) | 为 [GridCell](../../com.aspose.gridweb/gridcell) 设置公式。 |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | 设置公式及公式的值。 |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | 设置包含数据和一些格式的 HTML 字符串到此单元格。 |
| [setNumberType(int numbertype)](#setNumberType-int-) | 设置数字和日期的显示格式 |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | 获取单元格样式的副本。为单元格设置样式。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 获取此单元格中包含的值。 |
| [toString()](#toString--) | 返回表示当前 Cell 对象的字符串。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


指示此单元格是否包含外部链接。仅在单元格为公式单元格时适用。

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


从源单元格复制数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | 源 [GridCell](../../com.aspose.gridweb/gridcell) 对象。 |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


复制样式并为单元格设置样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | 源样式。 |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


为单元格创建评论对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 注释 | java.lang.String | 注释内容。 |
| 作者 | java.lang.String | 注释作者。 |
| isvisible | boolean | 注释是否可见。 |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


为单元格创建验证对象。

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype)。验证类型。 |
| isRequried | boolean | 单元格的值是否必填。 |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


检查此对象是否与另一个单元格对象引用相同的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 另一个 GridCell 对象 |

**Returns:**
布尔值 - 如果两个单元格对象引用同一单元格则为 true。
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


获取单元格中包含的布尔值。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


获取单元格的列号（从零开始）。

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


获取此单元格上的评论对象。

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


获取单元格中包含的 DateTime 值。

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


获取此单元格的格式化字符串值。

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


获取单元格中包含的 double 值。

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


获取单元格中包含的 float 值。

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


获取 [GridCell](../../com.aspose.gridweb/gridcell) 的公式。

**Remarks**

公式字符串总是以等号 (=) 开头。并且请始终使用逗号 (,) 作为参数分隔符，例如 "=SUM(A1, E1, H2)"。

用户可以在 Workbook 设计器文件中设置任意公式。Aspose.Cells 将保留所有公式。如果用户使用此属性为单元格设置公式，Workbook 内置函数的主要部分受到支持，且后续功能将陆续推出。如果您对 Workbook 内置函数有任何特殊需求，请告知我们。

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


获取包含此单元格数据和部分格式的 HTML 字符串。

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


获取单元格中包含的整数值。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取单元格的名称。例如：A1，F102。

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


获取单元格的行号（从零开始）。

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


获取单元格中包含的字符串值。

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


获取单元格样式的副本。为单元格设置样式。

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


返回单元格值类型，含义请参见 GridCellValueType.java。

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


获取此单元格中包含的值。

**Remarks**

可能的类型：

null，

Boolean，

DateTime，

Double，

Integer

String。

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


获取该值的宽度，单位为像素。

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为特定类型的哈希函数。

**Returns:**
int - 当前 GridCell 对象的哈希码。
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


检查公式是否能够正确计算结果。

**Remarks**

仅适用于公式单元格。

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


表示指定的单元格是否包含公式。

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


指示单元格的样式是否已设置。如果返回 false，则表示该单元格使用默认的单元格格式。

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




### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```


将布尔值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| param_boolean | boolean | 输入值 |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


将 DateTime 值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | 输入值 |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


将 double 值写入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| param_double | double | 输入值 |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


将一个 int 值放入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| param_int | int | 输入值 |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


将对象值放入单元格。相当于 setValue(Object param\_object)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objectValue | java.lang.Object | 输入值 |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


将一个 String 值放入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| param_string | java.lang.String | 输入值 |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


将字符串值写入单元格，并在适当时将其转换为其他数据类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringValue | java.lang.String | 输入值 |
| isConverted | boolean | True: 如适用，转换为其他数据类型。 |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


将值写入单元格，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringValue | java.lang.String | 输入值 |
| isConverted | boolean | True: 如适用，转换为其他数据类型。 |
| setStyle | boolean | True: 在转换为其他数据类型时将数字格式设置为单元格的样式 |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


使用字符串值设置单元格的值，并根据该值设置单元格格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringValue | java.lang.String | 输入值。 |

### removeComment() {#removeComment--}
```
public void removeComment()
```


移除单元格的注释对象。

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


移除单元格的验证对象。

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


为单元格设置边框（上、下、左、右），所有边框使用相同的边框样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | 边框样式。 |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


设置自定义格式，null 或空字符串表示没有自定义格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 自定义 | java.lang.String | 自定义字符串表示形式 |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


为 [GridCell](../../com.aspose.gridweb/gridcell) 设置公式。

**Remarks**

公式字符串总是以等号 (=) 开头。并且请始终使用逗号 (,) 作为参数分隔符，例如 "=SUM(A1, E1, H2)"。

用户可以在 Workbook 设计器文件中设置任意公式。Aspose.Cells 将保留所有公式。如果用户使用此属性为单元格设置公式，Workbook 内置函数的主要部分受到支持，且后续功能将陆续推出。如果您对 Workbook 内置函数有任何特殊需求，请告知我们。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


设置公式及公式的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String | 公式。 |
| 值 | java.lang.Object | 公式的值。 |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


设置包含数据和一些格式的 HTML 字符串到此单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


设置数字和日期的显示格式

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| numbertype | int | 该 numbertype 的值，参见 GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


获取单元格样式的副本。为单元格设置样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


获取此单元格中包含的值。

**Remarks**

可能的类型：

null，

Boolean，

DateTime，

Double，

Integer

String。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


返回表示当前 Cell 对象的字符串。

**Returns:**
java.lang.String -
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

