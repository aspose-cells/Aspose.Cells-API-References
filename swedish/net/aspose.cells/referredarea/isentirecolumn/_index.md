---
title: "ReferredArea.IsEntireColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskapen. Anger om detta område innehåller hela kolumnen"
type: docs
url: /sv/net/aspose.cells/referredarea/isentirecolumn/
---
## ReferredArea.IsEntireColumn property

Indikerar om detta område innehåller alla rader (hela kolumnen).

```csharp
public bool IsEntireColumn { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReferredAreaPropertyIsEntireColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Skapa ett namngivet intervall som refererar till hela kolumn B
            int index = workbook.Worksheets.Names.Add("PriceColumn");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!$B:$B";

            // Hämta det refererade området för det namngivna intervallet
            ReferredArea referredArea = workbook.Worksheets.Names["PriceColumn"].GetReferredAreas(false)[0];

            // Visa värdet för IsEntireColumn-egenskapen
            Console.WriteLine("IsEntireColumn value for PriceColumn: " + referredArea.IsEntireColumn);

            // Skapa ett annat namngivet intervall som refererar till ett specifikt intervall (inte hela kolumnen)
            int index2 = workbook.Worksheets.Names.Add("ProductRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1:$B$3";

            // Hämta det refererade området för det andra namngivna intervallet
            ReferredArea referredArea2 = workbook.Worksheets.Names["ProductRange"].GetReferredAreas(false)[0];

            // Visa värdet för IsEntireColumn-egenskapen för det andra intervallet
            Console.WriteLine("IsEntireColumn value for ProductRange: " + referredArea2.IsEntireColumn);

            // Demonstrera effekten av IsEntireColumn genom att kontrollera intervallens dimensioner
            Console.WriteLine("PriceColumn dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea.StartRow, referredArea.EndRow, referredArea.StartColumn, referredArea.EndColumn);

            Console.WriteLine("ProductRange dimensions: StartRow={0}, EndRow={1}, StartColumn={2}, EndColumn={3}",
                referredArea2.StartRow, referredArea2.EndRow, referredArea2.StartColumn, referredArea2.EndColumn);

            // Spara arbetsboken
            workbook.Save("ReferredAreaPropertyIsEntireColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


