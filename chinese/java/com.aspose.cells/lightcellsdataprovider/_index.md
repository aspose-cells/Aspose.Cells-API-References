---
title: "LightCellsDataProvider"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于在轻量模式下保存大型电子表格文件的数据提供程序。"
type: docs
url: /zh/java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

表示用于在轻量模式下保存大型电子表格文件的数据提供程序。

**Remarks**

使用此模式保存工作簿时，将在保存工作簿中的每个工作表时检查 [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-)。对于单个工作表，如果 [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) 返回 true，则该工作表的行/单元格的所有数据和属性将由此接口的实现提供。首先，将调用 [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) 获取要保存的下一行索引。如果返回有效的行索引（行索引必须按升序排列以便保存），则会通过 [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-) 提供表示该行的 Row 对象，以便实现设置其属性。对于一行，将首先检查 [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--)。如果返回有效的列索引（列索引必须按升序排列以便当前行的所有单元格），则会通过 [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) 提供表示该单元格的 Cell 对象，以便实现设置其数据和属性。在调用 [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) 后，该单元格将直接保存到生成的电子表格文件中。随后将检查并处理下一个单元格。

请注意，用户应仅更新由相应方法提供的当前 Row/Cell 对象的值和属性。因为单元格数据以流式方式写入结果文件，大多数其他对象可能已经写入结果文件，或已收集并写入了一些全局数据。因此，当用户在保存单元格数据时更新其他对象，这些操作可能无法影响已保存的数据。甚至更糟的是，这些操作可能导致不一致的数据被保存到结果文件，最终使文件损坏。因此，对于形状、列宽和样式、条件格式等所有其他对象，请不要在此实现的任何方法中操作它们。相反，请在调用 "Save" 方法之前管理它们并将其调整到最终状态。
## 方法

| 方法 | 描述 |
| --- | --- |
| [isGatherString()](#isGatherString--) | 检查单元格的当前字符串值是否需要收集到全局池中。 |
| [nextCell()](#nextCell--) | 获取下一个要保存的单元格。 |
| [nextRow()](#nextRow--) | 获取下一个要保存的行。 |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | 开始保存一个单元格的数据。 |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | 开始保存一行的数据。 |
| [startSheet(int sheetIndex)](#startSheet-int-) | 开始保存一个工作表。 |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


检查单元格的当前字符串值是否需要收集到全局池中。

**Remarks**

仅当此实现提供的单元格中存在大量重复的字符串值时，收集字符串值才有优势。在这种情况下，收集字符串可以节省大量内存并生成更小的结果文件。如果 LightCellsDataProvider 提供的单元格中有许多字符串值但相同的很少，收集字符串会消耗更多的内存和时间，并且对结果文件没有优势。

**Returns:**
boolean - 如果需要将字符串值收集到结果文件的全局池中，则为 true。
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


获取下一个要保存的单元格。

**Remarks**

它将在保存单个单元格开始时被调用。

**Returns:**
int - 要保存的下一个单元格的列索引。-1 表示已到达当前行数据的末尾，且没有进一步的单元格需要保存。
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


获取下一个要保存的行。

**Remarks**

它将在保存一行及其单元格数据开始时被调用（在 [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-) 之前）。

**Returns:**
int - 要保存的下一个行索引。-1 表示已到达当前工作表数据的末尾，且没有进一步的行需要保存。
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


开始保存一个单元格的数据。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | 用于实现填充数据的 Cell 对象。其列索引是最近一次调用 [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--) 返回的值。如果该单元格已在内部单元格模型中初始化，则使用已存在的 Cell 对象。否则，将使用临时 Cell 对象供实现填充数据。 |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


开始保存一行的数据。

**Remarks**

它将在保存一行及其单元格数据开始时被调用。如果当前行具有一些自定义属性，例如高度、样式等，实现应在此将这些属性设置到给定的 Row 对象上。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | 用于实现填充数据的 Row 对象。其行索引是最近一次调用 [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) 返回的值。如果该行已在内部单元格模型中初始化，则使用已存在的 Row 对象。否则，将使用临时 Row 对象供实现填充数据。 |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


开始保存一个工作表。

**Remarks**

它将在保存工作簿期间保存工作表开始时被调用。如果提供程序需要在 startRow(Row) 或 startCell(Cell) 方法中稍后引用 *`sheetIndex`*，即过程需要知道正在处理哪个工作表，则实现应在此保留 *`sheetIndex`* 的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 要保存的当前工作表的索引。 |

**Returns:**
boolean - 如果此提供程序将为给定工作表提供数据则为 true；如果给定工作表应使用其正常的数据模型（Cells）则为 false。
