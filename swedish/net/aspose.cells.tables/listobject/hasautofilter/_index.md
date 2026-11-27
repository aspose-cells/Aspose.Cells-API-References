---
title: "ListObject.HasAutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject‑egenskap. Anger om auto filter har tillämpats på denna tabell"
type: docs
url: /sv/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Anger om autofilter är tillämpat på den här tabellen.

```csharp
public bool HasAutoFilter { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för tabellen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Lägg till ett ListObject (tabell) som täcker dataintervallet
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // Säkerställ att tabellen storleksändras för att inkludera alla rader
                listObject.Resize(0, 0, 4, 2, true);

                // Läs och visa värdet för HasAutoFilter‑egenskapen
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // AutoFilter‑objektet kan nås via AutoFilter‑egenskapen
                // Visa att den inte är null när HasAutoFilter är true
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // Applicera ett enkelt filter på kolumnen "Score" (index 1) för att visa rader med Score >= 80
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Använd Cells.Rows för att kontrollera om raden är dold
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Rensa filtret
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Spara arbetsboken (valfritt)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


