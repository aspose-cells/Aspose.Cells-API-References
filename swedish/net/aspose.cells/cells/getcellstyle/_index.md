---
title: "Cells.GetCellStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämta stilen för angiven cell"
type: docs
url: /sv/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

Hämta stilen för given cell.

```csharp
public Style GetCellStyle(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | radindex |
| column | Int32 | column |

### Returvärde

stilen för angiven cell.

### Anmärkningar

Den returnerade stilen är endast den som är inställd för cellen eller ärvs från rad/kolumn för cellen, och inkluderar inte de tillämpade egenskaperna från andra inställningar såsom villkorlig formatering.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till cell B5 (rad 4, kolumn 1) och sätt initial stil
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // Skapa och tillämpa initial cellstil
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // Anropa GetCellStyle med Int32-parametrar (rad 4, kolumn 1)
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // Visa hämtade stilegenskaper
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // Ändra den hämtade stilen
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // Applicera den ändrade stilen tillbaka på cellen
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


