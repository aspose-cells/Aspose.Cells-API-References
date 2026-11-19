---
title: "WebWorksheet"
second_title: "Aspose.Cells for Java API 参考"
description: "表示一个 Web 工作表。"
type: docs
url: /zh/java/com.aspose.gridweb/webworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class WebWorksheet extends Control
```

表示一个 Web 工作表。

**Remarks**

注意：此类已过时。请改用 GridWorksheet。此类将在自 2014 年 8 月起 6 个月后被移除。Aspose 对您可能遇到的任何不便表示歉意。

**Example**

```
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WebWorksheet(MainWeb mw, GridWorksheet gwk)](#WebWorksheet-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | WebWorksheet 的构造函数。 |
| [WebWorksheet()](#WebWorksheet--) | WebWorksheet 的构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | 自动调整列宽。 |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | 自动调整列宽。 |
| [cancelNewBindRow()](#cancelNewBindRow--) | 取消并删除新添加的绑定行。 |
| [commitNewBindRow()](#commitNewBindRow--) | 提交新添加的绑定行并将其添加到数据源。 |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | 从另一个工作表对象复制。 |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | 为工作表设置数据源后，调用此方法自动生成绑定列。 |
| [createNewBindRow()](#createNewBindRow--) | 创建一个新的绑定行并绑定到数据源。 |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | 在工作表中创建小计。 |
| [dataBind()](#dataBind--) | 将工作表绑定到 DataSource。 |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | 删除一个绑定行。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | 在工作表中指定的单元格处冻结窗格。 |
| [getBindStartColumn()](#getBindStartColumn--) | 在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。 |
| [getBindStartRow()](#getBindStartRow--) | 在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。 |
| [getBindingSource()](#getBindingSource--) | 运行时实际绑定的数据源对象。 |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | 获取数据绑定模式下的绑定行数。 |
| [getDataMember()](#getDataMember--) | 从多成员 DataSource 获取 DataMember。 |
| [getDataSource()](#getDataSource--) | 获取 DataSource。 |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | 在数据绑定模式下，指示是否在工作表中创建绑定列标题。 |
| [getIndex()](#getIndex--) | 获取其在工作表集合中的索引。 |
| [getName()](#getName--) | 获取工作表的名称。 |
| [getUniqueID()](#getUniqueID--) | 获取控件中的唯一标识符。 |
| [getValidations()](#getValidations--) | 获取工作表中的数据验证设置集合。 |
| [getVisible()](#getVisible--) | 指示此工作表的名称是否显示在控件的工作表标签中。 |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | 对行进行分组。 |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | 对行进行分组。 |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | 获取工作表是否受保护。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | 使所有单元格可编辑。这是扩展属性。 |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | 使所有单元格只读。这是扩展属性，注意此属性在实际单元格中无法保留，如果想保持保护，请使用 setProtect。 |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | 在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。 |
| [setBindStartRow(int value)](#setBindStartRow-int-) | 在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。 |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | 获取数据绑定模式下的绑定行数。 |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | 从多成员 DataSource 设置 DataMember。 |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | 设置 DataSource。 |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | 使一组单元格可编辑。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 通过调用 SetAllCellsReadonly 方法将所有单元格设为只读。 |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | 在数据绑定模式下，指示是否在工作表中创建绑定列标题。 |
| [setName(String value)](#setName-java.lang.String-) | 设置工作表的名称。 |
| [setProtected(boolean value)](#setProtected-boolean-) | 设置工作表是否受保护。 |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | 将一组单元格设为只读。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 首先通过调用 SetAllCellsEditable 方法将所有单元格设为可编辑。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示此工作表的名称是否显示在控件的工作表标签中。 |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | 取消冻结工作表中的窗格。 |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | 取消分组行。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WebWorksheet(MainWeb mw, GridWorksheet gwk) {#WebWorksheet-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WebWorksheet(MainWeb mw, GridWorksheet gwk)
```


WebWorksheet 的构造函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

### WebWorksheet() {#WebWorksheet--}
```
public WebWorksheet()
```


WebWorksheet 的构造函数。

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


自动调整列宽。

**Remarks**

AutoFitColumn is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


自动调整列宽。此方法根据列中从 startRow 到 endRow 的单元格内容自动调整列宽。AutoFitColumn 是一个不精确的函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引，从零开始 |
| startRow | int | 起始行索引，零基 |
| endRow | int | 结束行索引，零基 |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


取消并删除新添加的绑定行。

**Returns:**
int - 行索引。如果没有新创建的绑定行，返回 -1。
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


提交新添加的绑定行并将其添加到数据源。

**Returns:**
int - 新行的行索引。如果未创建行，返回 -1。
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


从另一个工作表对象复制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | 另一张工作表。 |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


为工作表设置数据源后，调用此方法自动生成绑定列。

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


创建一个新的绑定行并绑定到数据源。

**Returns:**
int - 新行的行索引。如果未创建行，返回 -1。
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


在工作表中创建小计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnNameRowIndex | int | 列名行的行索引。 |
| dataRows | int | 数据行的数量。 |
| groupByColumnIndex | int | 要分组的列的列索引。 |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction)。小计函数类型。 |
| subtotalColumnIndexList | int[] | 需要进行小计的列索引。 |
| functionLabel | java.lang.String | 小计函数的标签。 |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | 总计行的样式。 |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | 小计行的样式。 |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype)。小计结果单元格的数字类型。 |
| customString | java.lang.String | 小计结果单元格的自定义格式字符串。可以为 null。 |

### dataBind() {#dataBind--}
```
public void dataBind()
```


将工作表绑定到 DataSource。

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


删除一个绑定行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowNum | int | 行索引。 |

**Returns:**
int - 被删除的行索引。如果没有删除绑定行，返回 -1。
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
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


在工作表中指定的单元格处冻结窗格。

**Remarks**

行索引和列索引不能全部为零。行数和列数也不能全部为零。

前两个参数指定冻结位置，后两个参数指定左上窗格中冻结的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |
| freezedRows | int | 顶部窗格中可见行数，不超过行索引。 |
| freezedColumns | int | 左侧窗格中可见列数，不超过列索引。 |

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


运行时实际绑定的数据源对象。当 DataSource 属性是 DataSet、DataTable 或 DataView 对象时，它是 DataView 对象。

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


获取数据绑定模式下的绑定行数。

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


从多成员 DataSource 获取 DataMember。通常它表示 DataSet 的 DataTable 对象。

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


获取 DataSource。通常它是 DataSet 对象。

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


在数据绑定模式下，指示是否在工作表中创建绑定列标题。

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取其在工作表集合中的索引。

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


获取工作表的名称。

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


获取控件中的唯一标识符。

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


获取工作表中的数据验证设置集合。

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


指示此工作表的名称是否显示在控件的工作表标签中。

**Returns:**
boolean
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


对行进行分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要分组的第一行索引。 |
| lastIndex | int | 要分组的最后一行索引。 |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


对行进行分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要分组的第一行索引。 |
| lastIndex | int | 要分组的最后一行索引。 |
| isHidden | boolean | 指定分组的行是否隐藏。 |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


获取工作表是否受保护。当工作表受保护时，除 IsLocked 属性为 false 的单元格外，所有单元格均不可编辑。

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




### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


使所有单元格可编辑。这是扩展属性。

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


使所有单元格只读。这是扩展属性，注意此属性在实际单元格中无法保留，如果想保持保护，请使用 setProtect。

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


在数据绑定模式下，BindStartRow 和 BindStartColumn 指示网格绑定到数据源的位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


获取数据绑定模式下的绑定行数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


从多成员 DataSource 设置 DataMember。通常它表示 DataSet 的 DataTable 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


设置 DataSource。通常它是 DataSet 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


将一系列单元格设为可编辑。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 通过调用 SetAllCellsReadonly 方法将所有单元格设为只读。然后调用此方法来指定要可编辑的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 范围的起始行。 |
| startColumn | int | 范围的起始列。 |
| 行 | int | 行的数量。 |
| 列 | int | 列的数量。 |

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


在数据绑定模式下，指示是否在工作表中创建绑定列标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置工作表的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


设置工作表是否受保护。当工作表受保护时，除 IsLocked 属性为 false 的单元格外，所有单元格均不可编辑。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


将一系列单元格设为只读。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 首先通过调用 SetAllCellsEditable 方法将所有单元格设为可编辑。然后调用此方法来指定要设为只读的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 范围的起始行。 |
| startColumn | int | 范围的起始列。 |
| 行 | int | 行的数量。 |
| 列 | int | 列的数量。 |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


指示此工作表的名称是否显示在控件的工作表标签中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


取消冻结工作表中的窗格。

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


取消分组行。

**Remarks**

仅删除外部组信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要取消分组的第一行索引。 |
| lastIndex | int | 要取消分组的最后一行索引。 |

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

