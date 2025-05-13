---
title: DataLabels.Area
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets the area
type: docs
url: /net/aspose.cells.charts/datalabels/area/
---
## DataLabels.Area property

Gets the `area`.

```csharp
public override Area Area { get; }
```

### Examples

```csharp
// Called: aseries1.DataLabels.Area.FillFormat.Pattern = FillPattern.Solid;
public void DataLabels_Property_Area()
{
    Console.WriteLine("DataLabels_Property_Area()");
    string outfn = Constants.destPath + "TEST_ChartDataLabelFill_out.xlsx";

    Workbook workbook = new Workbook();
    int sheetIndex = 0;

    Worksheet worksheet = workbook.Worksheets[sheetIndex];
    worksheet.Cells["A1"].PutValue(150);
    worksheet.Cells["A2"].PutValue(100);
    worksheet.Cells["A3"].PutValue(150);
    worksheet.Cells["B1"].PutValue(33);
    worksheet.Cells["B2"].PutValue(20);
    worksheet.Cells["B3"].PutValue(50);
    int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 15, 5);
    Chart chart = worksheet.Charts[chartIndex];
    chart.NSeries.Add("A1:B3", true);

    Series aseries1 = chart.NSeries[0];

    aseries1.DataLabels.ShowValue = true;
    aseries1.DataLabels.Area.FillFormat.Pattern = FillPattern.Solid;
    aseries1.DataLabels.Area.BackgroundColor = Color.White;

    workbook.Save(outfn);
}
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


