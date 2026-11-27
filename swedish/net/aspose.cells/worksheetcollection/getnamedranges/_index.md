---
title: "WorksheetCollection.GetNamedRanges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Hämtar alla fördefinierade namngivna områden i kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Hämtar alla fördefinierade namngivna områden i kalkylbladet.

```csharp
public Range[] GetNamedRanges()
```

### Returvärde

En array av Range-objekt. Om den definierade Namnets referens är extern eller har flera områden, kommer inget Range-objekt att returneras för detta Namn.

Returnerar null om det namngivna området inte finns.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa några namngivna områden för demonstration
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Anropa GetNamedRanges-metoden för att hämta alla namngivna områden
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Visa information om de namngivna områdena
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Spara arbetsboken
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


