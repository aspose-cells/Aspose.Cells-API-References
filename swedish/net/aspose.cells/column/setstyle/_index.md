---
title: "Column.SetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Column-metod. Anger stilen för den här kolumnen"
type: docs
url: /sv/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

Anger stilen för den här kolumnen.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | stilen som ska användas som standardstil för celler i den här kolumnen. |

### Anmärkningar

Denna metod anger endast den angivna stilen som standardstil för den här kolumnen, utan att ändra stilinställningarna för befintliga celler i kolumnen. För att uppdatera stilinställningarna för befintliga celler till den angivna stilen samtidigt, använd [`ApplyStyle`](../applystyle/)

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till den första kolumnen
            Column column = worksheet.Cells.Columns[0];

            // Skapa en ny stil från workbook
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // Applicera den anpassade stilen på hela kolumnen
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


