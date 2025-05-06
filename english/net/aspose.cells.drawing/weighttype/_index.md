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
// Called: AssertHelper.AreEqual(WeightType.MediumLine, aseries.Border.Weight, &amp;quot;chart.NSeries[0].Line.Weight&amp;quot;);
private void Type_WeightType(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            Series aseries = chart.NSeries[2];
            AssertHelper.AreEqual(WeightType.MediumLine, aseries.Border.Weight, &quot;chart.NSeries[0].Line.Weight&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


