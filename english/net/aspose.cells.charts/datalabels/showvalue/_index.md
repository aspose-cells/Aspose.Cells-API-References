---
title: DataLabels.ShowValue
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents a specified charts data label values display behavior. True displays the values. False to hide
type: docs
url: /net/aspose.cells.charts/datalabels/showvalue/
---
## DataLabels.ShowValue property

Represents a specified chart's data label values display behavior. True displays the values. False to hide.

```csharp
public bool ShowValue { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].DataLabels.ShowValue = true;
public void DataLabels_Property_ShowValue()
{
    Workbook workbook = new Workbook();
    workbook = TestLine.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.NSeries[0].DataLabels.ShowValue = true;
    chart.NSeries[0].DataLabels.Position = LabelPositionType.Right;

    checkLabelPositionType_Right(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkLabelPositionType_Right(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkLabelPositionType_Right(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


