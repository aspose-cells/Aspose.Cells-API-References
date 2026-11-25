---
title: "DataSorter.SortAsNumber"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. Indica se ordinare tutto ciò che sembra un numero"
type: docs
url: /it/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Indica se ordinare elementi che sembrano numeri.

```csharp
public bool SortAsNumber { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con numeri misti e numeri testuali
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Crea l'area di celle da ordinare
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // Crea un ordinatore di dati
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // Aggiungi chiave di ordinamento (colonna A)
            sorter.AddKey(idx, SortOrder.Ascending);

            // Ordina come numeri (true) o come stringhe (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Reimposta i dati per il secondo ordinamento
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Ordina come stringhe
            sorter.SortAsNumber = false;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("\nSorted as strings:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Vedi anche

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


