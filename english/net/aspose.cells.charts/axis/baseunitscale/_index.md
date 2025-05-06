---
title: Axis.BaseUnitScale
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the base unit scale for the category axis
type: docs
url: /net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Represents the base unit scale for the category axis.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Remarks

Setting this property only takes effect when the CategoryType property is set to TimeScale.

### Examples

```csharp
// Called: chart.CategoryAxis.BaseUnitScale = TimeUnit.Years;
[Test]
        public void Property_BaseUnitScale()
        {
            Workbook workbook = new Workbook();            
            workbook = new Workbook(Constants.sourcePath + &quot;Charts\\Column\\Book1.xls&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11)];
            chart.NSeries.Add(&quot;=Sheet1!$A$1:$B$10&quot;, true);
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Years;

            checkTimeUnit_Years(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkTimeUnit_Years(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkTimeUnit_Years(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


