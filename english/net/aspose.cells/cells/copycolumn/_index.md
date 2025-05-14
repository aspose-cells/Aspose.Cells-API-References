---
title: Cells.CopyColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of a whole column
type: docs
url: /net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Copies data and formats of a whole column.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |

### Examples

```csharp
// Called: cellsDest.CopyColumn(cellsSrc, 255, 0);
public void Cells_Method_CopyColumn()
{
    caseName = "testCopyColumn_Data_003";
    Workbook wbSrc = new Workbook();
    Cells cellsSrc = wbSrc.Worksheets[0].Cells;
    cellsSrc[0, 255].PutValue(1);
    cellsSrc[1, 255].PutValue(true);
    cellsSrc[2, 255].PutValue("abc");
    cellsSrc[3, 255].PutValue(false);
    cellsSrc[65535, 255].PutValue(2.56);

    Workbook wbDest = new Workbook();
    Cells cellsDest = wbDest.Worksheets[0].Cells;
    cellsDest.CopyColumn(cellsSrc, 255, 0);

    checkCopyColumn_Data_001(wbDest);
    wbDest.Save(Constants.destPath + "testCopyColumn.xls");
    wbDest = new Workbook(Constants.destPath + "testCopyColumn.xls");
    checkCopyColumn_Data_001(wbDest);
    wbDest.Save(Constants.destPath + "testCopyColumn.xlsx");
    wbDest = new Workbook(Constants.destPath + "testCopyColumn.xlsx");
    checkCopyColumn_Data_001(wbDest);
    wbDest.Save(Constants.destPath + "testCopyColumn.xml", SaveFormat.SpreadsheetML);
    wbDest = new Workbook(Constants.destPath + "testCopyColumn.xml");
    checkCopyColumn_Data_001(wbDest);
    wbDest.Save(Constants.destPath + "testCopyColumn.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


