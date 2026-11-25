---
title: "DataSorterKey.Color"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorterKey. Ottiene il colore ordinato"
type: docs
url: /it/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

Ottiene il colore ordinato.

```csharp
public Color Color { get; }
```

### Osservazioni

Ha effetto solo quando [`Type`](../type/) è CellColor o FontColor.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Crea un ordinatore di dati e aggiungi la chiave
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordina i dati
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Restituisci la proprietà colore dalle chiavi
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### Vedi anche

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


