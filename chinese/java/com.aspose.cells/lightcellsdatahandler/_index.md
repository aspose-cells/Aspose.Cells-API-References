---
title: "LightCellsDataHandler"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用于在轻量模式下读取大型电子表格文件的单元格数据处理器。"
type: docs
url: /zh/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

表示用于在轻量模式下读取大型电子表格文件的单元格数据处理器。

**Remarks**

使用此模式读取工作簿时，在读取工作簿中的每个工作表时会检查 [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-)。对于单个工作表，如果 [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) 返回 true，则该工作表的所有行/单元格的数据和属性将由此接口的实现进行检查和处理。对于每一行，会调用 [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) 来判断是否需要处理。如果需要处理该行，则首先读取该行的属性，用户可以通过 [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) 访问其属性。如果该行的单元格也需要处理，则 [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) 应返回 true，随后会为该行的每个现有单元格调用 [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) 以检查是否需要处理该单元格。如果需要处理某个单元格，则会调用 [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) 由接口实现来处理该单元格。

请注意，用户应仅操作由相应方法提供的当前 Row/Cell 对象的值和属性。由于单元格数据是以流式方式从模板文件读取的，其他大多数对象可能在单元格数据加载后被重置/更新。因此，在此实现中操作其他对象时，这些操作可能无法影响工作簿中已存在的对象。更糟的是，这些操作可能导致工作簿中的数据不一致，进而在以后引发意外问题或异常。因此，对于诸如形状、列宽和样式、条件格式等所有其他对象，请不要在此实现的任何方法中操作它们。相反，请在工作簿构建完成后再进行管理。
## 方法

| 方法 | 描述 |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | 开始处理一个单元格。 |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | 开始处理一行。 |
| [startCell(int columnIndex)](#startCell-int-) | 准备处理一个单元格。 |
| [startRow(int rowIndex)](#startRow-int-) | 准备处理一行。 |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | 开始处理一个工作表。 |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


开始处理一个单元格。

**Remarks**

在读取完一个单元格的数据后将被调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | 当前正在处理的单元格对象 |

**Returns:**
boolean - 是否需要将此单元格保留在当前工作表的单元格模型中。通常应为 false，以便在处理完后不在内存中保留所有单元格，从而节省内存。出于某些特殊目的，例如用户需要在整个工作簿处理完后仍访问某些单元格，用户可以让此方法返回 true，以将这些特殊单元格保留在 Cells 模型中，并通过诸如 Cells[row, column] 的 API 在以后访问它们。然而，将单元格数据保留在 Cells 模型中会占用更多内存，如果保留所有单元格，则在 LightCells 模式下读取模板文件将与普通方式读取相同。
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


开始处理一行。

**Remarks**

在读取完行的属性（如高度、样式等）后将被调用。但该行的单元格尚未读取。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | 当前正在处理的行对象。 |

**Returns:**
boolean - 是否需要处理此行的单元格。false 表示忽略该行的所有单元格。
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


准备处理一个单元格。

**Remarks**

在到达当前行的现有单元格时将被调用。当前行是上一次调用 [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) 时的行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 待处理单元格的列索引 |

**Returns:**
boolean - 是否需要处理此单元格。false 表示忽略该单元格并检查下一个，直至到达当前行单元格数据的末尾。
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


准备处理一行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 下一个待处理行的索引 |

**Returns:**
boolean - 是否需要处理此行（属性或单元格数据）。false 表示忽略该行及其单元格并检查下一行。
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


开始处理一个工作表。

**Remarks**

在读取工作表的单元格数据之前将被调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | 用于读取单元格数据的工作表。 |

**Returns:**
布尔值 - 指示是否需要处理此工作表的单元格数据。false 表示忽略此工作表。
