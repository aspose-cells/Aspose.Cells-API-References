---
title: "Cells.GetCellDisplayStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämta visningsstilen för angiven cell"
type: docs
url: /sv/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Hämta visningsstilen för given cell.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | radindex för angiven cell |
| column | Int32 | kolumn för angiven cell |

### Returvärde

visningsstilen för angiven cell.

### Anmärkningar

Samma med [`GetDisplayStyle`](../../cell/getdisplaystyle/), och samma med att använda SideBorders för `GetCellDisplayStyle`.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Förbered cellstil för demonstration
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // Skapa anpassad stil
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Applicera stil på cell
            cell.SetStyle(style);

            try
            {
                // Anropa GetCellDisplayStyle med rad 0 och kolumn 0
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // Egenskaper för visningsstil
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // Applicera visningsstilen på en annan cell för visuell verifiering
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Hämta visningsstilen för given cell.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | radindex för angiven cell |
| column | Int32 | kolumn för angiven cell |
| adjacentBorders | BorderType | Anger vilka kanter som måste kontrolleras och justeras enligt kanterna på intilliggande celler. Se beskrivningen för samma parameter i [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### Returvärde

visningsstilen för angiven cell.

### Anmärkningar

Om cellen också påverkas av andra inställningar såsom villkorsstyrd formatering, listobjekt osv., kan visningsstilen vara annorlunda än i [`GetCellStyle`](../getcellstyle/). Och eftersom dessa inställningar även kan tillämpas på tomma (icke‑existerande) celler, kan användning av denna metod undvika instansiering av dessa tomma celler, så prestandan blir bättre än att hämta Cell‑instansen från Cells och sedan anropa [`GetDisplayStyle`](../../cell/getdisplaystyle/).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till cell A1 och ange en kantstil
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // Anropa GetCellDisplayStyle med specifika parametrar (0,0 för A1, TopBorder-typ)
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // Kontrollera om den hämtade stilen matchar vår kantfärg
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // Demonstrera stilapplikation genom att modifiera en annan cell
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


