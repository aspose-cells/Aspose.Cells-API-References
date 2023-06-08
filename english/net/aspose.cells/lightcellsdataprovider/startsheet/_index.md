---
title: LightCellsDataProvider.StartSheet
second_title: Aspose.Cells for .NET API Reference
description: LightCellsDataProvider method. Starts to save a worksheet
type: docs
url: /net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Starts to save a worksheet.

```csharp
public bool StartSheet(int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | index of current sheet to be saved. |

### Return Value

true if this provider will provide data for the given sheet; false if given sheet should use its normal data model(Cells).

### Remarks

It will be called at the beginning of saving a worksheet during saving a workbook. If the provider needs to refer to

```csharp
sheetIndex
```

later in startRow(Row) or startCell(Cell) method, that is, if the process needs to know which worksheet is being processed, the implementation should retain the

```csharp
sheetIndex
```

value here.

### See Also

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


