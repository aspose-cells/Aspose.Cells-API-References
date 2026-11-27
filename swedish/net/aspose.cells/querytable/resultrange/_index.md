---
title: "QueryTable.ResultRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "QueryTable-egenskap. Hämtar resultatets område"
type: docs
url: /sv/net/aspose.cells/querytable/resultrange/
---
## QueryTable.ResultRange property

Hämtar intervallet för resultatet.

```csharp
public Range ResultRange { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyResultRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att simulera en frågetabell
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Kontrollera om det finns några frågetabeller i kalkylbladet
                if (worksheet.QueryTables.Count > 0)
                {
                    // Hämta den första frågetabellen
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Visa värdet för ResultRange-egenskapen (skrivskyddad operation)
                    Aspose.Cells.Range resultRange = queryTable.ResultRange;
                    Console.WriteLine("ResultRange Address: " + resultRange.Address);
                    Console.WriteLine("ResultRange Row Count: " + resultRange.RowCount);
                    Console.WriteLine("ResultRange Column Count: " + resultRange.ColumnCount);
                    Console.WriteLine("ResultRange First Row: " + resultRange.FirstRow);
                    Console.WriteLine("ResultRange First Column: " + resultRange.FirstColumn);

                    // Visa värdena i resultatområdet
                    Console.WriteLine("Values in ResultRange:");
                    foreach (Cell cell in resultRange)
                    {
                        Console.WriteLine($"Cell [{cell.Row}, {cell.Column}]: {cell.Value}");
                    }
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Spara arbetsboken
                workbook.Save("ResultRangeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


