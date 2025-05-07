---
title: DataLabels.SeparatorType
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets the separator type used for the data labels on a chart
type: docs
url: /net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Gets or sets the separator type used for the data labels on a chart.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Remarks

To set custom separator, please set the property `SeparatorType` as Custom and then specify the expected value for [`SeparatorValue`](../separatorvalue/).

### Examples

```csharp
// Called: chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Period;
[Test]
        public void Property_SeparatorType()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Period;
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            checkDataLablesSeparatorType_Period(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkDataLablesSeparatorType_Period(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkDataLablesSeparatorType_Period(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


