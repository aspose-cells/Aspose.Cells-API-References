---
title: Enum WeightType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.WeightType enum. Enumerates the weight types for a picture border or a chart line
type: docs
url: /net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Enumerates the weight types for a picture border or a chart line.

```csharp
public enum WeightType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| HairLine | `-1` | Represents the weight of hair line. |
| MediumLine | `1` | Represents the weight of medium line. |
| SingleLine | `0` | Represents the weight of single line. |
| WideLine | `2` | Represents the weight of wide line. |

### Examples

```csharp
// Called: AssertHelper.AreEqual(WeightType.WideLine, chartarea.Border.Weight, "chart.chartarea.Border.Weight");
private void Drawing_Type_WeightType(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(WeightType.WideLine, chartarea.Border.Weight, "chart.chartarea.Border.Weight");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


