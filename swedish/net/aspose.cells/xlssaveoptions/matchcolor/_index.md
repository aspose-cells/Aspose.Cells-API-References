---
title: "XlsSaveOptions.MatchColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsSaveOptions-egenskap. Anger om teckensnittsfärgen ska matchas eftersom det finns 56 färger i den standardfärgpaletten"
type: docs
url: /sv/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Anger om teckensnittsfärgen ska matchas eftersom det finns 56 färger i den standardfärgpaletten.

```csharp
public bool MatchColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Få åtkomst till cell B2 och ange text med specifik teckensnittsfärg
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // Ställ in teckensnittsfärgen till blå
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // Skapa sparalternativ med MatchColor satt till true
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // Spara arbetsboken med alternativen
            workbook.Save("output.xls", saveOptions);

            // Läs in den sparade filen igen för att verifiera att färgen bevarades
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // Verifiera att teckensnittsfärgen fortfarande är blå
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### Se även

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


