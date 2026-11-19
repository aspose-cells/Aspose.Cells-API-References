---
title: "BindColumn"
second_title: "Aspose.Cells for Java API 参考"
description: "绑定列。"
type: docs
url: /zh/java/com.aspose.gridweb/bindcolumn/
---

**Inheritance:**
java.lang.Object
```
public class BindColumn
```

绑定列。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [BindColumn()](#BindColumn--) | 默认构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeStyle()](#getAlternativeStyle--) | 获取列的替代样式。 |
| [getCaption()](#getCaption--) | 列的标题。 |
| [getClass()](#getClass--) |  |
| [getColumnHeaderStyle()](#getColumnHeaderStyle--) | 获取列的样式。 |
| [getCommandName()](#getCommandName--) | 列的命令名称。 |
| [getCommandText()](#getCommandText--) | 列的显示命令文本。 |
| [getCustomFormat()](#getCustomFormat--) | 自定义格式字符串。 |
| [getDataField()](#getDataField--) | 获取数据字段名称字符串。 |
| [getEnableSort()](#getEnableSort--) | 指示用户是否可以单击列标题以按此字段排序。 |
| [getImageUrl()](#getImageUrl--) | 命令超链接的图像 URL。 |
| [getName()](#getName--) | 仅在设计时使用。 |
| [getNumberType()](#getNumberType--) | 获取列的数字类型。 |
| [getStyle()](#getStyle--) | 获取列的样式。 |
| [getUseAlternativeStyle()](#getUseAlternativeStyle--) | 获取是否对列使用备用样式。 |
| [getValidation()](#getValidation--) | 获取列的验证对象。 |
| [getWidth()](#getWidth--) | 获取或设置列的宽度，仅接受像素或点。 |
| [hashCode()](#hashCode--) |  |
| [isAutoCreated()](#isAutoCreated--) | 指示列是否自动创建。 |
| [isReadOnly()](#isReadOnly--) | 指示列是否只读。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlternativeStyle(GridTableItemStyle value)](#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-) | 设置列的备用样式。 |
| [setAutoCreated(boolean value)](#setAutoCreated-boolean-) | 指示列是否自动创建。 |
| [setCaption(String value)](#setCaption-java.lang.String-) | 列的标题。 |
| [setColumnHeaderStyle(GridTableItemStyle value)](#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-) | 设置列的样式。 |
| [setCommandName(String value)](#setCommandName-java.lang.String-) | 列的命令名称。 |
| [setCommandText(String value)](#setCommandText-java.lang.String-) | 列的显示命令文本。 |
| [setCustomFormat(String value)](#setCustomFormat-java.lang.String-) | 自定义格式字符串。 |
| [setDataField(String value)](#setDataField-java.lang.String-) | 设置数据字段名称字符串。 |
| [setEnableSort(boolean value)](#setEnableSort-boolean-) | 指示用户是否可以单击列标题以按此字段排序。 |
| [setImageUrl(String value)](#setImageUrl-java.lang.String-) | 命令超链接的图像 URL。 |
| [setNumberType(int value)](#setNumberType-int-) | 设置列的数字类型。 |
| [setReadOnly(boolean value)](#setReadOnly-boolean-) | 指示列是否只读。 |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | 设置列的样式。 |
| [setUseAlternativeStyle(boolean value)](#setUseAlternativeStyle-boolean-) | 设置是否对列使用备用样式。 |
| [setValidation(GridValidation value)](#setValidation-com.aspose.gridweb.GridValidation-) | 设置列的验证对象。 |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | 获取或设置列的宽度，仅接受像素或点。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### BindColumn() {#BindColumn--}
```
public BindColumn()
```


默认构造函数。

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
### getAlternativeStyle() {#getAlternativeStyle--}
```
public GridTableItemStyle getAlternativeStyle()
```


获取列的替代样式。

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCaption() {#getCaption--}
```
public String getCaption()
```


列的标题。

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnHeaderStyle() {#getColumnHeaderStyle--}
```
public GridTableItemStyle getColumnHeaderStyle()
```


获取列的样式。

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getCommandName() {#getCommandName--}
```
public String getCommandName()
```


列的命令名称。如果设置了 CommandName 属性，将在绑定的单元格中创建 CellCommand 超链接。

**Returns:**
java.lang.String
### getCommandText() {#getCommandText--}
```
public String getCommandText()
```


列的显示命令文本。如果设置为 null，单元格将使用字段值作为命令文本。

**Returns:**
java.lang.String
### getCustomFormat() {#getCustomFormat--}
```
public String getCustomFormat()
```


自定义格式字符串。

**Returns:**
java.lang.String
### getDataField() {#getDataField--}
```
public String getDataField()
```


获取数据字段名称字符串。

**Returns:**
java.lang.String
### getEnableSort() {#getEnableSort--}
```
public boolean getEnableSort()
```


指示用户是否可以单击列标题以按此字段排序。

**Returns:**
boolean
### getImageUrl() {#getImageUrl--}
```
public String getImageUrl()
```


命令超链接的图像 URL。

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


仅在设计时使用。

**Returns:**
java.lang.String
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


获取列的数字类型。

参见 [NumberType](../../com.aspose.gridweb/numbertype)。

**Returns:**
int
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


获取列的样式。

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUseAlternativeStyle() {#getUseAlternativeStyle--}
```
public boolean getUseAlternativeStyle()
```


获取是否对列使用备用样式。

**Returns:**
boolean
### getValidation() {#getValidation--}
```
public GridValidation getValidation()
```


获取列的验证对象。

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


获取或设置列的宽度，仅接受像素或点。

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoCreated() {#isAutoCreated--}
```
public boolean isAutoCreated()
```


指示列是否自动创建。如果为 true，则在设计时用户更改数据源时，列将被删除。

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


指示列是否只读。

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




### setAlternativeStyle(GridTableItemStyle value) {#setAlternativeStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setAlternativeStyle(GridTableItemStyle value)
```


设置列的备用样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoCreated(boolean value) {#setAutoCreated-boolean-}
```
public void setAutoCreated(boolean value)
```


指示列是否自动创建。如果为 true，则在设计时用户更改数据源时，列将被删除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


列的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setColumnHeaderStyle(GridTableItemStyle value) {#setColumnHeaderStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setColumnHeaderStyle(GridTableItemStyle value)
```


设置列的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setCommandName(String value) {#setCommandName-java.lang.String-}
```
public void setCommandName(String value)
```


列的命令名称。如果设置了 CommandName 属性，将在绑定的单元格中创建 CellCommand 超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCommandText(String value) {#setCommandText-java.lang.String-}
```
public void setCommandText(String value)
```


列的显示命令文本。如果设置为 null，单元格将使用字段值作为命令文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCustomFormat(String value) {#setCustomFormat-java.lang.String-}
```
public void setCustomFormat(String value)
```


自定义格式字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDataField(String value) {#setDataField-java.lang.String-}
```
public void setDataField(String value)
```


设置数据字段名称字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setEnableSort(boolean value) {#setEnableSort-boolean-}
```
public void setEnableSort(boolean value)
```


指示用户是否可以单击列标题以按此字段排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setImageUrl(String value) {#setImageUrl-java.lang.String-}
```
public void setImageUrl(String value)
```


命令超链接的图像 URL。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


设置列的数字类型。

参见 [NumberType](../../com.aspose.gridweb/numbertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setReadOnly(boolean value) {#setReadOnly-boolean-}
```
public void setReadOnly(boolean value)
```


指示列是否只读。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


设置列的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setUseAlternativeStyle(boolean value) {#setUseAlternativeStyle-boolean-}
```
public void setUseAlternativeStyle(boolean value)
```


设置是否对列使用备用样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setValidation(GridValidation value) {#setValidation-com.aspose.gridweb.GridValidation-}
```
public void setValidation(GridValidation value)
```


设置列的验证对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridValidation](../../com.aspose.gridweb/gridvalidation) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


获取或设置列的宽度，仅接受像素或点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

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

