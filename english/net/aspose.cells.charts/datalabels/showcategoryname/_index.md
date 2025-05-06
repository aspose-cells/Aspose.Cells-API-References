---
title: DataLabels.ShowCategoryName
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents a specified charts data label category name display behavior.True to display the category name for the data labels on a chart. False to hide
type: docs
url: /net/aspose.cells.charts/datalabels/showcategoryname/
---
## DataLabels.ShowCategoryName property

Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide.

```csharp
public bool ShowCategoryName { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].DataLabels.ShowCategoryName = true;
[Test]
        public void Property_ShowCategoryName()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.NewLine;
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            checkDataLablesSeparatorType_NewLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkDataLablesSeparatorType_NewLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkDataLablesSeparatorType_NewLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


