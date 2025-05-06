---
title: Cells.CopyRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of a whole row
type: docs
url: /net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Copies data and formats of a whole row.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |

### Examples

```csharp
// Called: cellsDest.CopyRow(cellsSrc, 3, 0);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testCopyRow_Style_003&quot;;
            Workbook wbSrc = new Workbook();            
            wbSrc = new Workbook(Constants.sourcePath + &quot;insertDelete\\testStyle.xls&quot;);
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;

            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;
            cellsDest.CopyRow(cellsSrc, 3, 0);
            cellsDest.CopyRow(cellsSrc, 7, 2);

            checkCopyRow_Style_003(wbDest);
            wbDest.Save(Constants.destPath + &quot;testCopyRow.xls&quot;);
            wbDest = new Workbook(Constants.destPath + &quot;testCopyRow.xls&quot;);
            checkCopyRow_Style_003(wbDest);
            wbDest.Save(Constants.destPath + &quot;testCopyRow.xlsx&quot;);
            wbDest = new Workbook(Constants.destPath + &quot;testCopyRow.xlsx&quot;);
            checkCopyRow_Style_003(wbDest);
            wbDest.Save(Constants.destPath + &quot;testCopyRow.xml&quot;, SaveFormat.SpreadsheetML);
            wbDest = new Workbook(Constants.destPath + &quot;testCopyRow.xml&quot;);
            checkCopyRow_Style_003(wbDest);
            wbDest.Save(Constants.destPath + &quot;testCopyRow.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


