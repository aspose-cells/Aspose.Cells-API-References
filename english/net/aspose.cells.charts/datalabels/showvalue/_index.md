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
[Test]
        public void Property_ShowValue()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            checkDataLablesSeparatorType_Comma(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkDataLablesSeparatorType_Comma(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkDataLablesSeparatorType_Comma(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


