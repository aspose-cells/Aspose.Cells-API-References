---
title: "AutoFilter.Refresh"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Uppdatera autofilter för att dölja eller visa raderna"
type: docs
url: /sv/net/aspose.cells/autofilter/refresh/
---
## Refresh() {#refresh}

Uppdatera autofilter för att dölja eller visa raderna.

```csharp
public int[] Refresh()
```

### Returvärde

Returnerar index för alla dolda rader.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["B6"].PutValue("Header1");
            worksheet.Cells["C6"].PutValue("Header2");
            worksheet.Cells["D6"].PutValue("Header3");
            worksheet.Cells["E6"].PutValue("Values");
            
            for (int i = 7; i <= 15; i++)
            {
                worksheet.Cells["B" + i].PutValue("Item " + (i-6));
                worksheet.Cells["E" + i].PutValue((i-6) * 100);
            }

            // Applicera autofilter
            worksheet.AutoFilter.Range = "B6:E6";
            
            // Filtrera värden större än 500
            worksheet.AutoFilter.Custom(3, FilterOperatorType.GreaterThan, 500);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
            
            // Ändra filter för att visa värden lika med 500 eller större än 700
            worksheet.AutoFilter.Custom(3, FilterOperatorType.Equal, 500, false, FilterOperatorType.GreaterThan, 700);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("After refresh - Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("After refresh - Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Refresh(bool) {#refresh_1}

Hämtar alla dolda raders index.

```csharp
public int[] Refresh(bool hideRows)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| hideRows | Boolean | Om true, dölj de filtrerade raderna. |

### Returvärde

Returnerar index för alla dolda rader.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(1);
            worksheet.Cells["A5"].PutValue(3);
            
            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.AddFilter(0, "1"); // Filter to show only rows with value 1
            
            // Uppdatera filtret och hämta dolda rader
            int[] hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("Hidden rows after filter:");
            if (hiddenRows != null)
            {
                foreach (int row in hiddenRows)
                {
                    Console.WriteLine(row);
                }
            }
            
            // Visa all data och uppdatera igen
            worksheet.AutoFilter.ShowAll();
            hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("\nHidden rows after showing all:");
            if (hiddenRows == null)
            {
                Console.WriteLine("No hidden rows");
            }
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


