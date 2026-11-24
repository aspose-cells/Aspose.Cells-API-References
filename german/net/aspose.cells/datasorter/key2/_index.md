---
title: "DataSorter.Key2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataSorter‑Eigenschaft. Stellt den Index der zweiten sortierten Spalte dar, absolute Position: Spalte A ist 0, B ist 1"
type: docs
url: /de/net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Gibt den Index der zweitens sortierten Spalte an (absolute Position, Spalte A ist 0, B ist 1, ...).

```csharp
public int Key2 { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey2Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // DataSorter erstellen und Eigenschaften setzen
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.Key1 = 0; // Sort by first column (Name)
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key2 = 1; // Then sort by second column (Age)
            sorter.Order2 = SortOrder.Descending;

            // Datenbereich sortieren
            sorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Die sortierten Daten ausgeben, um die Verwendung von Key2 zu demonstrieren
            Console.WriteLine("Sorted Data:");
            for (int i = 0; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### Siehe auch

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


