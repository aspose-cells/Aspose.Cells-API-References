---
title: "AutoFilter.RemoveFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Tar bort ett filter för en filterkolumn"
type: docs
url: /sv/net/aspose.cells/autofilter/removefilter/
---
## RemoveFilter(int, string) {#removefilter_1}

Tar bort ett filter för en filterkolumn.

```csharp
public void RemoveFilter(int fieldIndex, string criteria)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| kriterier | String | Det angivna kriteriet (en sträng; till exempel "101"). Det kan endast vara null eller vara ett av cellernas värden i den här kolumnen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodRemoveFilterWithInt32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för demonstration
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["C1"].PutValue("Price");
            
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["C2"].PutValue(999.99);
            
            worksheet.Cells["A3"].PutValue("Novel");
            worksheet.Cells["B3"].PutValue("Books");
            worksheet.Cells["C3"].PutValue(19.99);
            
            worksheet.Cells["A4"].PutValue("Smartphone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["C4"].PutValue(599.99);

            // Ställ in autofilterintervall (rubriker + 3 datarader)
            worksheet.AutoFilter.SetRange(0, 0, 2);

            try
            {
                AutoFilter autoFilter = worksheet.AutoFilter;
                
                // Tillämpa filter på kolumnen Category (fieldIndex 1) för "Electronics"
                autoFilter.AddFilter(1, "Electronics");
                autoFilter.Refresh(); // Apply filter to hide non-matching rows
                
                // Ta bort det specifika filtret från kolumnen Category
                autoFilter.RemoveFilter(1, "Electronics");
                autoFilter.Refresh(); // Re-apply filter (now shows all rows)

                Console.WriteLine("RemoveFilter executed: Electronics filter removed from Category column.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("AutoFilterMethodRemoveFilterWithInt32StringDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveFilter(int) {#removefilter}

Ta bort det specifika filtret.

```csharp
public void RemoveFilter(int fieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det specifika filterindexet |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveFilterWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Lägg till ett filter
            filter.AddFilter(0, "Apple");
            filter.Refresh();
            
            Console.WriteLine("After adding filter - Visible rows:");
            PrintVisibleRows(worksheet);
            
            // Ta bort filtret
            filter.RemoveFilter(0);
            filter.Refresh();
            
            Console.WriteLine("\nAfter removing filter - Visible rows:");
            PrintVisibleRows(worksheet);
        }
        
        private static void PrintVisibleRows(Worksheet worksheet)
        {
            for (int i = 0; i < worksheet.Cells.MaxDataRow + 1; i++)
            {
                if (!worksheet.Cells.Rows[i].IsHidden)
                {
                    Console.WriteLine($"Row {i + 1}: {worksheet.Cells[i, 0].StringValue}");
                }
            }
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


