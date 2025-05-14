---
title: Chart.SubTitle
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts subtitle. Only for ODS format file
type: docs
url: /net/aspose.cells.charts/chart/subtitle/
---
## Chart.SubTitle property

Gets the chart's sub-title. Only for ODS format file.

```csharp
public Title SubTitle { get; }
```

### Examples

```csharp
// Called: string s1 = chart1.SubTitle.Text;
public void Chart_Property_SubTitle()
{
    string path = Constants.sourcePath + "Charts/Other/";
    Workbook book1 = new Workbook(path + "example.xlsx");
    Chart chart1 = book1.Worksheets[0].Charts[0];
    string s1 = chart1.SubTitle.Text;
    Assert.AreEqual(null, s1);
    Workbook book2 = new Workbook(path + "example.ods");
    Chart chart2 = book2.Worksheets[0].Charts[0];
    string s2 = chart2.SubTitle.Text;
    Assert.AreEqual("SubTitle1", s2);
}
```

### See Also

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


