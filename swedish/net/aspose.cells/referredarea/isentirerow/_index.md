---
title: "ReferredArea.IsEntireRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskap. Anger om detta område innehåller alla kolumner eller hela raden"
type: docs
url: /sv/net/aspose.cells/referredarea/isentirerow/
---
## ReferredArea.IsEntireRow property

Indikerar om detta område innehåller alla kolumner (hela raden).

```csharp
public bool IsEntireRow { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Skapa ett namngivet område som refererar till hela rad 2
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$2:$2";

            // Hämta det refererade området för det namngivna intervallet
            ReferredArea referredArea = workbook.Worksheets.Names["NamedRange1"].GetReferredAreas(false)[0];

            // Visa det aktuella värdet av IsEntireRow
            Console.WriteLine("IsEntireRow value for NamedRange1: " + referredArea.IsEntireRow);

            // Skapa ett annat namngivet intervall som refererar till ett specifikt intervall (inte hela raden)
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Hämta det refererade området för det andra namngivna intervallet
            ReferredArea referredArea2 = workbook.Worksheets.Names["NamedRange2"].GetReferredAreas(false)[0];

            // Visa det aktuella värdet av IsEntireRow för det andra intervallet
            Console.WriteLine("IsEntireRow value for NamedRange2: " + referredArea2.IsEntireRow);

            // Demonstrera effekten av IsEntireRow genom att kontrollera intervallens dimensioner
            Console.WriteLine("NamedRange1 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("NamedRange2 dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Spara arbetsboken
            workbook.Save("ReferredAreaPropertyIsEntireRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


