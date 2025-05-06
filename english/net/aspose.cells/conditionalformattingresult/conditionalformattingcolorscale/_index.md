---
title: ConditionalFormattingResult.ConditionalFormattingColorScale
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingResult property. Gets the ColorScale object
type: docs
url: /net/aspose.cells/conditionalformattingresult/conditionalformattingcolorscale/
---
## ConditionalFormattingResult.ConditionalFormattingColorScale property

Gets the ColorScale object.

```csharp
public ColorScale ConditionalFormattingColorScale { get; }
```

### Examples

```csharp
// Called: ColorScale colorScale = cfr.ConditionalFormattingColorScale;
public static void Property_ConditionalFormattingColorScale()
        {
            // Instantiate a workbook object
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

            // Set ColorScale properties
            fc.ColorScale.Is3ColorScale = true;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxColor = Color.Green;

            // Apply some values to the cells
            for (int i = 0; i &lt;= 10; i++)
            {
                for (int j = 0; j &lt;= 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Get the conditional formatting result for a specific cell
            Cell cell = worksheet.Cells[&quot;A1&quot;];
            ConditionalFormattingResult cfr = cell.GetConditionalFormattingResult();

            // Access the properties of ConditionalFormattingResult
            Style conditionalStyle = cfr.ConditionalStyle;
            ConditionalFormattingIcon icon = cfr.ConditionalFormattingIcon;
            DataBar dataBar = cfr.ConditionalFormattingDataBar;
            ColorScale colorScale = cfr.ConditionalFormattingColorScale;
            Color colorScaleResult = cfr.ColorScaleResult;

            // Display some of the properties
            Console.WriteLine(&quot;Conditional Style Background Color: &quot; + (conditionalStyle != null ? conditionalStyle.BackgroundColor : Color.Empty));
            Console.WriteLine(&quot;Conditional Formatting Icon Type: &quot; + (icon != null ? icon.Type.ToString() : &quot;No Icon&quot;));
            Console.WriteLine(&quot;Conditional Formatting DataBar Color: &quot; + (dataBar != null ? dataBar.Color.ToString() : &quot;No DataBar&quot;));
            Console.WriteLine(&quot;Conditional Formatting ColorScale Min Color: &quot; + (colorScale != null ? colorScale.MinColor.ToString() : &quot;No ColorScale&quot;));
            Console.WriteLine(&quot;Color Scale Result: &quot; + colorScaleResult);

            // Save the workbook
            workbook.Save(&quot;ConditionalFormattingResultExample.xlsx&quot;);
            workbook.Save(&quot;ConditionalFormattingResultExample.pdf&quot;);
        }
```

### See Also

* class [ColorScale](../../colorscale/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


