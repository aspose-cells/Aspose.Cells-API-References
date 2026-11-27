---
title: "SmartTagCollection.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagCollection-egenskap. Hämtar kolumnen för cellens smarttaggar"
type: docs
url: /sv/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

Hämtar kolumnen för cellens smarta taggar.

```csharp
public int Column { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en smarttagg i cell C5 (rad 4, kolumn 2)
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // Hämta SmartTagCollection för cell C5
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Visa kolumnen för cellen som innehåller dessa smarttaggar
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // Lägg till ytterligare en smarttagg i cell E2 (rad 1, kolumn 4) för att demonstrera en annan kolumn
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // Spara arbetsboken
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


