---
title: "CellsHelper.GetUsedColors"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Hämtar alla använda färger i arbetsboken"
type: docs
url: /sv/net/aspose.cells/cellshelper/getusedcolors/
---
## CellsHelper.GetUsedColors method

Hämtar alla använda färger i arbetsboken.

```csharp
public static Color[] GetUsedColors(Workbook workbook)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arbetsbok | Arbetsbok | Arbetsboksobjektet. |

### Returvärde

De använda färgerna.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några färgade celler för att demonstrera de använda färgerna
            worksheet.Cells["A1"].PutValue("Red Cell");
            worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
            worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());

            worksheet.Cells["B1"].PutValue("Blue Cell");
            worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
            worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());

            worksheet.Cells["C1"].PutValue("Green Cell");
            worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
            worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());

            try
            {
                // Anropa GetUsedColors-metoden med arbetsbok-parameter
                Color[] usedColors = CellsHelper.GetUsedColors(workbook);

                // Visa de använda färgerna
                Console.WriteLine("Used colors in the workbook:");
                foreach (Color color in usedColors)
                {
                    Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


