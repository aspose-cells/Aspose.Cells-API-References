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
[Test, Ignore(&quot;Not ready to test this yet&quot;)]
        public void Method_Range_()
        {
            caseName = &quot;testRangeCopyData_Formual_Excel2007&quot;;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\testformual2.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range rangeSrc = cells.CreateRange(1, 1, 1, 12);
            Aspose.Cells.Range rangeDest = cells.CreateRange(1048575, 16372, 1, 12);
            rangeDest.CopyData(rangeSrc);

            checkRangeCopyData_Formual_Excel2007(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopyData.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testRangeCopyData.xlsx&quot;);
            checkRangeCopyData_Formual_Excel2007(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopyData.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testRangeCopyData.xml&quot;);
            checkRangeCopyData_Formual_Excel2007(workbook);
            workbook.Save(Constants.destPath + &quot;testRangeCopyData.xls&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


