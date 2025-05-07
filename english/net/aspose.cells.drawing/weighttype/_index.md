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
// Called: chartarea.Border.Weight = WeightType.HairLine;
[Test]
        public void Type_WeightType()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            chartarea.Border.Weight = WeightType.HairLine;

            checkWeightType_HairLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkWeightType_HairLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkWeightType_HairLine(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


