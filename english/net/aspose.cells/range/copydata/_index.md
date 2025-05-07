---
title: Range.CopyData
second_title: Aspose.Cells for .NET API Reference
description: Range method. Copies cell data including formulas from a source range
type: docs
url: /net/aspose.cells/range/copydata/
---
## Range.CopyData method

Copies cell data (including formulas) from a source range.

```csharp
public void CopyData(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |

### Examples

```csharp
// Called: rangeDest.CopyData(rangeSrc);
[Test, Ignore("Not ready to test this yet")]
        public void Method_Range_()
        {
            caseName = "testRangeCopyData_Formual_002";
            Workbook workbook = new Workbook(Constants.sourcePath + "Copy//copy_002.xls");
            Worksheet sheetSrc = workbook.Worksheets[0];
            Cells cellsSrc = sheetSrc.Cells;
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "sheetDest";
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(65531, 251, 5, 5);
            rangeDest.CopyData(rangeSrc);

            checkRangeCopyData_Formual_002(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xls");
            workbook = new Workbook(Constants.destPath + "testRangeCopyData.xls");
            checkRangeCopyData_Formual_002(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xlsx");
            workbook = new Workbook(Constants.destPath + "testRangeCopyData.xlsx");
            checkRangeCopyData_Formual_002(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testRangeCopyData.xml");
            checkRangeCopyData_Formual_002(workbook);
            workbook.Save(Constants.destPath + "testRangeCopyData.xls");
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


