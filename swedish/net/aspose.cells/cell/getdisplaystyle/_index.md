---
title: "Cell.GetDisplayStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar visningsstilen för denna cell"
type: docs
url: /sv/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Hämtar cellens visningsstil.

```csharp
public Style GetDisplayStyle()
```

### Returvärde

visningsstil för denna cell

### Anmärkningar

Samma sak gäller vid användning av SideBorders för `GetDisplayStyle`. Det vill säga, den här metoden kommer att kontrollera och justera topp-/botten-/vänster-/högerkanter för denna cell enligt stilen ([`GetStyle`](../getstyle/)) för dess angränsande celler, men kontrollerar inte de sammanslagna cellerna och kontrollerar inte visningsstilen för angränsande celler.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange stil för cell A1
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // Ange stil för cell A23
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // Hämta och visa stilar
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
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

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Hämtar cellens visningsstil.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| includeMergedBorders | Boolean | Anger om kantkontroller av sammanslagna celler. |

### Returvärde

visningsstil för denna cell

### Anmärkningar

Om den angivna flaggan är falsk är den samma som `GetDisplayStyle`. Annars är den samma som att använda SideBorders&#x7C;DynamicStyleBorders för `GetDisplayStyle`.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Få åtkomst till cell B2 och ange några stilinställningar.
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // Hämta visningsstil med formatering (true-parameter).
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // Skriv ut den högra kantlinjens stil.
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
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

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Hämtar cellens visningsstil.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| adjacentBorders | BorderType | Anger vilka kanter som behöver kontrolleras och justeras enligt kanterna på intilliggande celler. |

### Returvärde

visningsstil för denna cell

### Anmärkningar

Om den här cellen också påverkas av andra inställningar såsom villkorsstyrd formatering, listobjekt osv., kan visningsstilen skilja sig från [`GetStyle`](../getstyle/). För flaggor som justerar kanter enligt intilliggande celler indikerar TopBorder/BottomBorder/LeftBorder/RightBorder om man ska kontrollera och kombinera respektive nedre/övre/höger/vänster kant på de celler som ligger till vänster/höger/övre/nedre intill denna. Av prestanda- och kompatibilitetsskäl används vissa uppräkningar för att beteckna speciella operationer: Horizontal/Vertical anger om man ska kontrollera och kombinera den nedre/högra kanten på sammanslagna celler till denna. Diagonal (det vill säga både DiagonalUpBorder och DiagonalDownBorder har satts) betyder att man kontrollerar och kombinerar kanter från visningsstilen för intilliggande celler. Observera att kontroll av kanter/stilar för intilliggande celler, särskilt visningsstilar, är en tidskrävande process. Om det inte behövs att hämta kanterna för den returnerade stilen, ger användning av None för att inaktivera processen för intilliggande celler bättre prestanda. När kanter hämtas från intilliggande celler enbart baserat på de stilar som definierats på dessa celler (utan att sätta Diagonal) kan prestandan också bli bättre eftersom kontroll av en cells visningsstil också är tidskrävande.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ange exempeldata
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Skapa villkorlig formatering
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Hämta visningsstil med olika kanttyper.
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### Se även

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


