---
title: Range.CopyStyle
second_title: Aspose.Cells for .NET API Reference
description: Range method. Copies style settings from a source range
type: docs
url: /net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Copies style settings from a source range.

```csharp
public void CopyStyle(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |

### Examples

```csharp
// Called: rangeDest.CopyStyle(rangeSrc);
[Test, Ignore("Not ready to test this yet")]
        public void Method_Range_()
        {
            caseName = "testRangeCopyStyle_MergedCells";
            Workbook workbook = new Workbook(Constants.sourcePath + "Copy\\mergedCells_003.xls");
            Worksheet sheetSrc = workbook.Worksheets[0];
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "sheetDest";
            Cells cellsSrc = sheetSrc.Cells;
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(7, 5, 10, 3);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(7, 5, 10, 3);
            rangeDest.CopyStyle(rangeSrc);

            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xls");
            workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xls");
            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xlsx");
            workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xlsx");
            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xml", SaveFormat.SpreadsheetML);
             workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xml");
            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyStyle.xls");
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


