---
title: "DataSorter.Key3"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. Rappresenta l'indice della terza colonna ordinata; la posizione assoluta della colonna A è 0, B è 1"
type: docs
url: /it/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

Rappresenta l'indice della terza colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...).

```csharp
public int Key3 { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // Crea un ordinatore di dati
            DataSorter sorter = workbook.DataSorter;
            
            // Ordina per Punteggio (decrescente), poi per Nome (crescente), poi per Voto (decrescente)
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // Ordina l'intervallo di dati
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // Salva la cartella di lavoro
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


