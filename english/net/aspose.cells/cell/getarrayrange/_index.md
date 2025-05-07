---
title: Cell.GetArrayRange
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the array range if the cells formula is an array formula
type: docs
url: /net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Gets the array range if the cell's formula is an array formula.

```csharp
public CellArea GetArrayRange()
```

### Return Value

The array range.

### Remarks

Only applies when the cell's formula is an array formula

### Examples

```csharp
// Called: CellArea ca = cell.GetArrayRange();
[Test]
        public void Method_GetArrayRange()
        {
            Workbook wbSrc = new Workbook(Constants.sourcePath + "CellsNet44755_Src.xlsm");
            Workbook wbCopyBase = new Workbook(Constants.sourcePath + "CellsNet44755_CopyBase.xlsm");
            //<- Working
            Worksheet testSheetSrc = wbSrc.Worksheets["TestSheet"];
            Worksheet testSheetCopyBase = wbCopyBase.Worksheets["TestSheet"];

            Aspose.Cells.Range sourceRange = testSheetCopyBase.Cells.CreateRange(13, 1, true);
            Aspose.Cells.Range tgtRange = testSheetSrc.Cells.CreateRange(3, 1, true);
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            tgtRange.Copy(sourceRange, options);
            Cell cell = testSheetSrc.Cells["D107"];
            CellArea ca = cell.GetArrayRange();
            Assert.AreEqual(106, ca.StartRow);
            Assert.AreEqual(3, ca.StartColumn);
            Util.ReSave(wbSrc, SaveFormat.Xlsm);
            //wbSrc.Save(Constants.destPath + "CellsNet44755.xlsm");
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


