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
public void Range_Method_CopyData()
{
    caseName = "testRangeCopyData_Picture";
    Workbook workbook = new Workbook(Constants.sourcePath + "insertDelete\\testPicture.xls");
    Worksheet sheetSrc = workbook.Worksheets[0];
    Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
    sheetDest.Name = "sheetDest";
    Cells cellsSrc = sheetSrc.Cells;
    Cells cellsDest = sheetDest.Cells;
    Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("B3", "B3");
    Aspose.Cells.Range rangeDest = cellsDest.CreateRange("B3", "B3");
    rangeDest.CopyData(rangeSrc);

    checkRangeCopyData_Picture(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyData.xls");
    workbook = new Workbook(Constants.destPath + "testRangeCopyData.xls");
    checkRangeCopyData_Picture(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyData.xlsx");
    workbook = new Workbook(Constants.destPath + "testRangeCopyData.xlsx");
    checkRangeCopyData_Picture(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyData.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testRangeCopyData.xml");
    checkRangeCopyData_Picture(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyData.xls");
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


