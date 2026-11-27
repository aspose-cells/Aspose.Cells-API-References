---
title: "Cell.GetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar cellens stil"
type: docs
url: /sv/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Hämtar cellstilen.

```csharp
public Style GetStyle()
```

### Returvärde

Stilobjekt.

### Anmärkningar

För att ändra cellens stil, anropa metoden Cell.SetStyle() efter att du har modifierat det returnerade stilobjektet. Denna metod är samma som `GetStyle` med sant värde för parametern.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange olika vertikala justeringar för celler
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // Demonstrera GetStyle()-metoden
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

Om checkBorders är true, kontrollera om andra cellers kanter kommer att påverka stilen för den här cellen.

```csharp
public Style GetStyle(bool checkBorders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| checkBorders | Boolean | Kontrollera andra cellers kanter |

### Returvärde

Stilobjekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till en cell och ange några exempeldata
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // Hämta cellens stil utan att ärva från rad/kolumn (false-parameter)
            Style style = cell.GetStyle(false);
            
            // Modifiera stilen
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // Applicera den modifierade stilen på cellen
            cell.SetStyle(style);

            // Verifiera stilförändringarna
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


