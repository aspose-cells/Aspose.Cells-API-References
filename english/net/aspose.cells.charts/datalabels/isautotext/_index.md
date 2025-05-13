---
title: DataLabels.IsAutoText
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Indicates the text is auto generated
type: docs
url: /net/aspose.cells.charts/datalabels/isautotext/
---
## DataLabels.IsAutoText property

Indicates the text is auto generated.

```csharp
public override bool IsAutoText { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(point.DataLabels.IsAutoText);
// Mo Shujun Bug
public void DataLabels_Property_IsAutoText()
{
    Console.WriteLine("DataLabels_Property_IsAutoText()");
    string infn = path + @"example.xlsx";
    //string outfn = path + @"example.xlsx";

    Workbook workbook = new Workbook(infn);
    Worksheet worksheet = workbook.Worksheets[1];
    Chart chart = worksheet.Charts[1];
    Assert.AreEqual("10K80ME-C9.1-TI", chart.Title.Text);
    foreach (Series ser in chart.NSeries)
    {
        foreach (ChartPoint point in ser.Points)
        {
            Console.WriteLine(point.DataLabels.IsAutoText);
            Console.WriteLine(point.DataLabels.Text);
        }
    }
    Util.ReSave(workbook, SaveFormat.Xlsx);
}
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


