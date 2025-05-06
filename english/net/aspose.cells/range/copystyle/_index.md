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
[Test, Ignore(&quot;Not ready to test this yet&quot;)]
        public void Method_Range_()
        {
            caseName = &quot;testRangeCopyStyle_MergedCells&quot;;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Copy\\mergedCells_003.xls&quot;);
            Worksheet sheetSrc = workbook.Worksheets[0];
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = &quot;sheetDest&quot;;
            Cells cellsSrc = sheetSrc.Cells;
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(7, 5, 10, 3);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(7, 5, 10, 3);
            rangeDest.CopyStyle(rangeSrc);

            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopyStyle.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testRangeCopyStyle.xls&quot;);
            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopyStyle.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testRangeCopyStyle.xlsx&quot;);
            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopyStyle.xml&quot;, SaveFormat.SpreadsheetML);
             workbook = new Workbook(Constants.destPath + &quot;testRangeCopyStyle.xml&quot;);
            checkRangeCopyStyle_MergedCells(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopyStyle.xls&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


