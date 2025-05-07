---
title: Enum FillType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.FillType enum. Fill format type
type: docs
url: /net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Fill format type.

```csharp
public enum FillType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Represents automatic formatting type. |
| None | `1` | Represents none formatting type. |
| Solid | `2` | Solid fill format. |
| Gradient | `3` | Gradient fill format. |
| Texture | `4` | Texture fill format(includes picture fill). |
| Pattern | `5` | Pattern fill format. |
| Group | `6` | Inherit the fill properties of the group. |

### Examples

```csharp
// Called: AssertHelper.AreEqual(FillType.Automatic, chartarea.Area.FillFormat.FillType, "chartarea.Area.FillFormat.GradientColorType");
private void Type_FillType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(FillType.Automatic, chartarea.Area.FillFormat.FillType, "chartarea.Area.FillFormat.GradientColorType");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


