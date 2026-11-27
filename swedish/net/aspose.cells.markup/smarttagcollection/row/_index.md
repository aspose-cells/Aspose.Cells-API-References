---
title: "SmartTagCollection.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagCollection-egenskap. Hämtar raden för cellens smarta taggar"
type: docs
url: /sv/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

Hämtar raden för cellens smarta taggar.

```csharp
public int Row { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en smart tag i cell A1 (rad 0, kolumn 0)
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // Hämta SmartTagCollection för cell A1
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Visa raden för cellen som innehåller dessa smarta taggar
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // Obs: Row-egenskapen är skrivskyddad, så vi kan inte sätta den
            // smartTags.Row = 5; // Detta skulle orsaka ett kompileringsfel

            // Lägg till en annan smart tag i cell B3 (rad 2, kolumn 1) för att demonstrera en annan rad
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // Spara arbetsboken
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


