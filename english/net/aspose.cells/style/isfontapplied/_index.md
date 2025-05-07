---
title: Style.IsFontApplied
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicate whether the font formatting should be applied
type: docs
url: /net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Indicate whether the font formatting should be applied.

```csharp
public bool IsFontApplied { get; set; }
```

### Remarks

Only for named style.

### Examples

```csharp
// Called: style.IsFontApplied = true;
public static void Property_IsFontApplied()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access a cell from the worksheet
            Cell cell = worksheet.Cells["A1"];
            
            // Get the style of the cell
            Style style = cell.GetStyle();
            
            // Set various properties of the style
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Set the style to the cell
            cell.SetStyle(style);
            
            // Save the workbook
            workbook.Save("StyleExample.xlsx");
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


