---
title: "Workbook.CustomTheme"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Anpassar temat"
type: docs
url: /sv/net/aspose.cells/workbook/customtheme/
---
## Workbook.CustomTheme method

Anpassar temat.

```csharp
public void CustomTheme(string themeName, Color[] colors)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| themeName | String | Temanamn |
| färger | Color[] | Temats färger |

### Anmärkningar

Längden på färgerna bör vara 12.

| **Array-index** | **Tematyp** |
| --- | --- |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Hyperlänk |
| 11 | Följd hyperlänk |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class WorkbookMethodCustomThemeWithStringColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för att demonstrera temaeffekter
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Demonstration");
            var style = cell.GetStyle();
            style.Font.IsBold = true;
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Förbered temafärger
            Color[] customColors = new Color[]
            {
                Color.FromArgb(255, 0, 0),     // Red
                Color.FromArgb(0, 255, 0),     // Green
                Color.FromArgb(0, 0, 255),     // Blue
                Color.FromArgb(255, 255, 0),    // Yellow
                Color.FromArgb(255, 0, 255),    // Magenta
                Color.FromArgb(0, 255, 255),    // Cyan
                Color.FromArgb(128, 0, 128),    // Purple
                Color.FromArgb(128, 128, 0),   // Olive
                Color.FromArgb(0, 128, 128),    // Teal
                Color.FromArgb(128, 0, 0),      // Maroon
                Color.FromArgb(0, 128, 0),     // Green (dark)
                Color.FromArgb(0, 0, 128)       // Navy
            };

            try
            {
                // Tillämpa anpassat tema
                workbook.CustomTheme("MyCustomTheme", customColors);

                // Skapa en formaterad cell för att demonstrera temaeffekt
                var themedCell = worksheet.Cells["A3"];
                themedCell.PutValue("Themed Text");
                var themedStyle = workbook.CreateStyle();
                themedStyle.Font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0);
                themedStyle.Font.Size = 12;
                themedCell.SetStyle(themedStyle);

                // Spara arbetsboken
                workbook.Save("CustomThemeDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error applying custom theme: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


