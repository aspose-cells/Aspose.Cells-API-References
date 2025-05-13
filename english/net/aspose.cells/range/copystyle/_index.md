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
public void Range_Method_CopyStyle()
{
    caseName = "testRangeCopyStyle_Style_PatternSetting";
    Workbook workbook = new Workbook(Constants.sourcePath + "Copy\\testPatternSetting.xls");
    Worksheet sheetSrc = workbook.Worksheets[0];
    Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
    sheetDest.Name = "sheetDest";
    Cells cellsSrc = sheetSrc.Cells;
    Cells cellsDest = sheetDest.Cells;
    Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(1, 1, 11, 5);
    Aspose.Cells.Range rangeDest = cellsDest.CreateRange(1, 1, 11, 5);
    rangeDest.CopyStyle(rangeSrc);

    checkRangeCopyStyle_Style_PatternSetting(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyStyle.xls");
    workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xls");
    checkRangeCopyStyle_Style_PatternSetting(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyStyle.xlsx");
    workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xlsx");
    checkRangeCopyStyle_Style_PatternSetting(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyStyle.xml", SaveFormat.SpreadsheetML);
     workbook = new Workbook(Constants.destPath + "testRangeCopyStyle.xml");
    checkRangeCopyStyle_Style_FontSetting(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyStyle.xls");
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


