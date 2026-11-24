---
title: "AutoFilter.Refresh"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Aktualisiert AutoFilter, um Zeilen auszublenden oder wieder einzublenden"
type: docs
url: /de/net/aspose.cells/autofilter/refresh/
---
## Refresh() {#refresh}

Aktualisiere AutoFilter, um Zeilen auszublenden oder wieder einzublenden.

```csharp
public int[] Refresh()
```

### Rückgabewert

Gibt die Indizes aller ausgeblendeten Zeilen zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["B6"].PutValue("Header1");
            worksheet.Cells["C6"].PutValue("Header2");
            worksheet.Cells["D6"].PutValue("Header3");
            worksheet.Cells["E6"].PutValue("Values");
            
            for (int i = 7; i <= 15; i++)
            {
                worksheet.Cells["B" + i].PutValue("Item " + (i-6));
                worksheet.Cells["E" + i].PutValue((i-6) * 100);
            }

            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "B6:E6";
            
            // Werte filtern, die größer als 500 sind
            worksheet.AutoFilter.Custom(3, FilterOperatorType.GreaterThan, 500);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
            
            // Filter ändern, um Werte anzuzeigen, die gleich 500 oder größer als 700 sind
            worksheet.AutoFilter.Custom(3, FilterOperatorType.Equal, 500, false, FilterOperatorType.GreaterThan, 700);
            worksheet.AutoFilter.Refresh();
            
            Console.WriteLine("After refresh - Row 7 hidden: " + worksheet.Cells.IsRowHidden(7));
            Console.WriteLine("After refresh - Row 13 hidden: " + worksheet.Cells.IsRowHidden(13));
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Refresh(bool) {#refresh_1}

Liest die Indizes aller ausgeblendeten Zeilen.

```csharp
public int[] Refresh(bool hideRows)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| hideRows | Boolean | Wenn true, die gefilterten Zeilen ausblenden. |

### Rückgabewert

Gibt alle Indizes ausgeblendeter Zeilen zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRefreshWithBooleanDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(1);
            worksheet.Cells["A5"].PutValue(3);
            
            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:A5";
            worksheet.AutoFilter.AddFilter(0, "1"); // Filter to show only rows with value 1
            
            // Filter aktualisieren und ausgeblendete Zeilen erhalten
            int[] hiddenRows = worksheet.AutoFilter.Refresh(false);
            
            Console.WriteLine("Hidden rows after filter:");
            if (hiddenRows != null)
            {
                foreach (int row in hiddenRows)
                {
                    Console.WriteLine(row);
                }
            }
            
            // Alle Daten anzeigen und erneut aktualisieren
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

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


