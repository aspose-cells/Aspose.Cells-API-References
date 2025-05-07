---
title: Range.CopyValue
second_title: Aspose.Cells for .NET API Reference
description: Range method. Copies cell value from a source range
type: docs
url: /net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Copies cell value from a source range.

```csharp
public void CopyValue(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |

### Examples

```csharp
// Called: rangeDest.CopyValue(rangeSrc);
[Test]
        public void Method_Range_()
        {
            caseName = "testRangeCopyValue_HideRowAndColumn";
            Workbook workbook = new Workbook();            
            workbook = new Workbook(Constants.sourcePath + "Copy\\hide_001.xls");
            Worksheet sheetSrc = workbook.Worksheets[0];
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "sheetDest";
            Cells cellsSrc = sheetSrc.Cells;
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(2, 0, 9, 5);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(2, 0, 9, 5);
            rangeDest.CopyValue(rangeSrc);

            checkRangeCopyValue_HideRowAndColumn(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyValue.xls");           
            workbook = new Workbook(Constants.destPath + "testRangeCopyValue.xls");
            checkRangeCopyValue_HideRowAndColumn(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyValue.xlsx");            
            workbook = new Workbook(Constants.destPath + "testRangeCopyValue.xlsx");
            checkRangeCopyValue_HideRowAndColumn(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyValue.xml", SaveFormat.SpreadsheetML);            
            workbook = new Workbook(Constants.destPath + "testRangeCopyValue.xml");
            checkRangeCopyValue_HideRowAndColumn(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyValue.xls");
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


