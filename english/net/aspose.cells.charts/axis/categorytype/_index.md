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
// Called: AssertHelper.AreEqual(CategoryType.AutomaticScale, chart.CategoryAxis.CategoryType, &amp;quot;chart.CategoryAxis.CategoryType&amp;quot;);
private void Property_CategoryType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet1&quot;];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(CategoryType.AutomaticScale, chart.CategoryAxis.CategoryType, &quot;chart.CategoryAxis.CategoryType&quot;);
        }
```

### See Also

* enum [CategoryType](../../categorytype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


