---
title: "FontConfigs.DefaultFontName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-egenskap. Hämtar eller anger standardteckensnittsnamnet"
type: docs
url: /sv/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

Hämtar eller anger standardteckensnittets namn.

```csharp
public static string DefaultFontName { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa det aktuella standardteckensnittsnamnet
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // Ställ in ett nytt standardteckensnittsnamn
            FontConfigs.DefaultFontName = "Arial";

            // Skapa en stil utan explicit teckensnitt för att demonstrera användning av standardteckensnitt
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // Spara arbetsboken för att se effekten
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // Verifiera att teckensnittet tillämpades korrekt
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### Se även

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


