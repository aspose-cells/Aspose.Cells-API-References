---
title: ColorScale.MidColor
second_title: Aspose.Cells for .NET API Reference
description: ColorScale property. Get or set the gradient color for the middle value in the range
type: docs
url: /net/aspose.cells/colorscale/midcolor/
---
## ColorScale.MidColor property

Get or set the gradient color for the middle value in the range.

```csharp
public Color MidColor { get; set; }
```

### Examples

```csharp
// Called: fc.ColorScale.MidColor = Color.Yellow;
public static void Property_MidColor()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Sets the conditional format range
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Adds condition
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Setting properties for ColorScale
            fc.ColorScale.Is3ColorScale = true;

            // Setting min value
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Setting mid value
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Setting max value
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Save the workbook
            workbook.Save(&quot;ConditionalFormattingValueExample.xlsx&quot;);
            workbook.Save(&quot;ConditionalFormattingValueExample.pdf&quot;);
            return;
        }
```

### See Also

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


