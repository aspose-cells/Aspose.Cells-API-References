---
title: "Style.IsFontApplied"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om teckensnittsformatering ska tillämpas"
type: docs
url: /sv/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Anger om teckensnittsformateringen ska tillämpas.

```csharp
public bool IsFontApplied { get; set; }
```

### Anmärkningar

Endast för namngiven stil.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till en cell från kalkylbladet
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // Hämta stil för cellen
            Style style = cell.GetStyle();
            
            // Använd teckensnittsinställningar
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // Aktivera teckensnittstillämpning
            style.IsFontApplied = true;
            
            // Ställ in den modifierade stilen tillbaka i cellen
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


