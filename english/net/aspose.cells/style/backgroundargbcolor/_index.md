---
title: Style.BackgroundArgbColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the background color with a 32bit ARGB value
type: docs
url: /net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

Gets and sets the background color with a 32-bit ARGB value.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Examples

```csharp
// Called: style.BackgroundArgbColor = Color.Yellow.ToArgb();
public static void Property_BackgroundArgbColor()
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


