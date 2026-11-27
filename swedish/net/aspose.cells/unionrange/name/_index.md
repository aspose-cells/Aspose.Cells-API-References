---
title: "UnionRange.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑egenskap. Hämtar eller anger namnet på området"
type: docs
url: /sv/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Hämtar eller anger namnet på området.

```csharp
public string Name { get; set; }
```

### Anmärkningar

Namngivet intervall stöds. Till exempel,

range.Name = "Sheet1!MyRange";

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // Skapa områden och kombinera dem till ett unionområde
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Visa det aktuella värdet på Name‑egenskapen
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // Ange ett nytt namn för union‑området
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // Visa att namnet kan ändras igen
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // Spara arbetsboken
                workbook.Save("UnionRangeNameDemo.xlsx");
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

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


