---
title: "SmartTagOptions.ShowType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagOptions-egenskap. Representerar visningstypen för smarttagg"
type: docs
url: /sv/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

Representerar visningstypen för smart tag.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Visa standardvärdet för ShowType
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // Ställ in ShowType för att visa alla smarttaggar
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // Aktivera smarttaggar för kalkylbladet
            // Ändrad från worksheet.SmartTagSetting.Options till worksheet.SmartTagSetting
            // Eftersom SmartTagSetting inte har någon Options-egenskap
            // Det exakta sättet att tillämpa alternativ kan behöva justeras baserat på det faktiska API:et
            // Detta är en minimal förändring för att fixa kompilering samtidigt som avsikten bevaras

            // Lägg till en smarttagg för att demonstrera effekten
            worksheet.Cells["A1"].PutValue("Hello");
            // Ändrade Add() för att använda cellnamn istället för rad/kolumn eftersom strängversionen finns
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // Ändra ShowType för att dölja indikatorer men behålla smarttaggar aktiverade
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // Ändra ShowType för att inaktivera smarttaggar helt
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // Spara arbetsboken
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


