---
title: "DataSorter.Key2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. Rappresenta l'indice della seconda colonna ordinata; posizione assoluta, la colonna A è 0, B è 1"
type: docs
url: /it/net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Rappresenta l'indice della seconda colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

```csharp
public int Key2 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey2Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Crea DataSorter e imposta le proprietà
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.Key1 = 0; // Sort by first column (Name)
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key2 = 1; // Then sort by second column (Age)
            sorter.Order2 = SortOrder.Descending;

            // Ordina l'intervallo di dati
            sorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Emetti i dati ordinati per dimostrare l'uso di Key2
            Console.WriteLine("Sorted Data:");
            for (int i = 0; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### Vedi anche

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


