---
title: "Column.GetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Column-metod. Hämtar stilen för den här kolumnen."
type: docs
url: /sv/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Hämtar stilen för den här kolumnen.

```csharp
public Style GetStyle()
```

### Anmärkningar

Att ändra det returnerade stilobjektet direkt har ingen effekt för denna kolumn eller några celler i den här kolumnen. Du måste anropa [`ApplyStyle`](../applystyle/) eller [`SetStyle`](../setstyle/)‑metoden för att tillämpa ändringen på denna kolumn. Kolumnens stil är den stil som ärvs av celler i den här kolumnen (de celler som saknar anpassade stilinställningar, såsom befintliga celler som inte har fått stil explicit, eller de som ännu inte har instansierats).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange stil för kolumn 5
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // Ställ in stil för rad 7
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // Verifiera kolumnstil
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // Verifiera radstil
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // Spara arbetsboken
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


