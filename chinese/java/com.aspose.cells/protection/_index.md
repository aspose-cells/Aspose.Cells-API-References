---
title: "保护"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表可用的各种保护选项类型。"
type: docs
url: /zh/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

表示工作表可用的各种保护选项类型。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | 复制保护信息。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | 表示在受保护的工作表上是否允许删除列。 |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | 表示在受保护的工作表上是否允许删除行。 |
| [getAllowEditingContent()](#getAllowEditingContent--) | 表示在受保护的工作表上是否允许用户编辑已锁定单元格的内容。 |
| [getAllowEditingObject()](#getAllowEditingObject--) | 表示在受保护的工作表上是否允许用户操作绘图对象。 |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | 表示在受保护的工作表上是否允许用户编辑方案。 |
| [getAllowFiltering()](#getAllowFiltering--) | 表示在工作表受保护之前创建的 AutoFilter 是否允许用户使用。 |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | 表示在受保护的工作表上是否允许对单元格进行格式设置。 |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | 表示在受保护的工作表上是否允许对列进行格式设置 |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | 表示在受保护的工作表上是否允许对行进行格式设置 |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | 表示在受保护的工作表上是否允许插入列 |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | 表示在受保护的工作表上是否允许插入超链接 |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | 表示在受保护的工作表上是否允许插入行 |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | 表示在受保护的工作表上是否允许用户选择已锁定的单元格。 |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | 表示在受保护的工作表上是否允许用户选择未锁定的单元格。 |
| [getAllowSorting()](#getAllowSorting--) | 表示在受保护的工作表上是否允许使用排序选项。 |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | 表示在受保护的工作表上是否允许用户操作数据透视表。 |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | 表示用于保护工作表的密码。 |
| [getPasswordHash()](#getPasswordHash--) | 获取当前密码的哈希值。 |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | 指示工作表是否已使用密码受保护。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | 表示在受保护的工作表上是否允许删除列。 |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | 表示在受保护的工作表上是否允许删除行。 |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | 表示在受保护的工作表上是否允许用户编辑已锁定单元格的内容。 |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | 表示在受保护的工作表上是否允许用户操作绘图对象。 |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | 表示在受保护的工作表上是否允许用户编辑方案。 |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | 表示在工作表受保护之前创建的 AutoFilter 是否允许用户使用。 |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | 表示在受保护的工作表上是否允许对单元格进行格式设置。 |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | 表示在受保护的工作表上是否允许对列进行格式设置 |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | 表示在受保护的工作表上是否允许对行进行格式设置 |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | 表示在受保护的工作表上是否允许插入列 |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | 表示在受保护的工作表上是否允许插入超链接 |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | 表示在受保护的工作表上是否允许插入行 |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | 表示在受保护的工作表上是否允许用户选择已锁定的单元格。 |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | 表示在受保护的工作表上是否允许用户选择未锁定的单元格。 |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | 表示在受保护的工作表上是否允许使用排序选项。 |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | 表示在受保护的工作表上是否允许用户操作数据透视表。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 表示用于保护工作表的密码。 |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | 验证密码。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


复制保护信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


表示在受保护的工作表上是否允许删除列。

**Remarks**

当工作表受保护时，包含要删除单元格的列必须是未锁定的，并且必须启用"Select unlocked cells"选项。

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


表示在受保护的工作表上是否允许删除行。

**Remarks**

当工作表受保护时，包含要删除单元格的行必须是未锁定的，并且必须启用"Select unlocked cells"选项。

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


表示在受保护的工作表上是否允许用户编辑已锁定单元格的内容。

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


表示在受保护的工作表上是否允许用户操作绘图对象。

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


表示在受保护的工作表上是否允许用户编辑方案。

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


表示在工作表受保护之前创建的 AutoFilter 是否允许用户使用。

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


表示在受保护的工作表上是否允许对单元格进行格式设置。

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


表示在受保护的工作表上是否允许对列进行格式设置

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


表示在受保护的工作表上是否允许对行进行格式设置

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


表示在受保护的工作表上是否允许插入列

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


表示在受保护的工作表上是否允许插入超链接

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


表示在受保护的工作表上是否允许插入行

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


表示在受保护的工作表上是否允许用户选择已锁定的单元格。

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


表示在受保护的工作表上是否允许用户选择未锁定的单元格。

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


表示在受保护的工作表上是否允许使用排序选项。

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


表示在受保护的工作表上是否允许用户操作数据透视表。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


表示用于保护工作表的密码。

**Remarks**

如果密码设置为 null 或空字符串，则可以在不使用密码的情况下取消保护工作表或工作簿。否则，必须指定密码才能取消保护工作表或工作簿。

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


获取当前密码的哈希值。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


指示工作表是否已使用密码受保护。

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




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


表示在受保护的工作表上是否允许删除列。

**Remarks**

当工作表受保护时，包含要删除单元格的列必须是未锁定的，并且必须启用"Select unlocked cells"选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


表示在受保护的工作表上是否允许删除行。

**Remarks**

当工作表受保护时，包含要删除单元格的行必须是未锁定的，并且必须启用"Select unlocked cells"选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


表示在受保护的工作表上是否允许用户编辑已锁定单元格的内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


表示在受保护的工作表上是否允许用户操作绘图对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


表示在受保护的工作表上是否允许用户编辑方案。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


表示在工作表受保护之前创建的 AutoFilter 是否允许用户使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


表示在受保护的工作表上是否允许对单元格进行格式设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


表示在受保护的工作表上是否允许对列进行格式设置

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


表示在受保护的工作表上是否允许对行进行格式设置

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


表示在受保护的工作表上是否允许插入列

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


表示在受保护的工作表上是否允许插入超链接

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


表示在受保护的工作表上是否允许插入行

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


表示在受保护的工作表上是否允许用户选择已锁定的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


表示在受保护的工作表上是否允许用户选择未锁定的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


表示在受保护的工作表上是否允许使用排序选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


表示在受保护的工作表上是否允许用户操作数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


表示用于保护工作表的密码。

**Remarks**

如果密码设置为 null 或空字符串，则可以在不使用密码的情况下取消保护工作表或工作簿。否则，必须指定密码才能取消保护工作表或工作簿。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


验证密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 密码 | java.lang.String | 密码。 |

**Returns:**
boolean -
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

