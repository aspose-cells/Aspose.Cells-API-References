---
title: Axis.CategoryType
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the category axis type
type: docs
url: /net/aspose.cells.charts/axis/categorytype/
---
## Axis.CategoryType property

Represents the category axis type.

```csharp
public CategoryType CategoryType { get; set; }
```

### Examples

```csharp
// Called: chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
private void Property_CategoryType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\Column\\Book1.xls");
            Worksheet sheet = workbook.Worksheets["Sheet1"];
            Chart chart = sheet.Charts[sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11)];
            chart.NSeries.Add("=Sheet1!$A$1:$B$10", true);
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;

            checkCategoryType_TimeScale(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkCategoryType_TimeScale(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkCategoryType_TimeScale(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [CategoryType](../../categorytype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


