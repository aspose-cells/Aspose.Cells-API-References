---
title: "CustomFilterCollection.And"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Egenskapen CustomFilterCollection. Anger om de två kriterierna har ett och-förhållande"
type: docs
url: /sv/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

Indikerar om de två kriterierna har ett \"och\"‑förhållande.

```csharp
public bool And { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Skapa en ny CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Visa standardvärdet för And‑egenskapen
                Console.WriteLine($"Default And property value: {filters.And}");

                // Ställ in And‑egenskapen till true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // Ställ in And‑egenskapen till false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Spara arbetsboken
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


