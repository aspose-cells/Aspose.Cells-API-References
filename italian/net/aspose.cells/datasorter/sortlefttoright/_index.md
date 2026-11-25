---
title: "DataSorter.SortLeftToRight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorter. True indica che l'orientamento dell'ordinamento è da sinistra a destra. False indica che l'orientamento dell'ordinamento è dall'alto verso il basso. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True indica che l'orientamento dell'ordinamento è da sinistra a destra. False indica che l'orientamento dell'ordinamento è dall'alto verso il basso. Il valore predefinito è false.

```csharp
public bool SortLeftToRight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio (le colonne saranno trattate come righe quando SortLeftToRight=true)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // Crea un ordinatore di dati e impostalo per ordinare da sinistra a destra
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // Imposta la chiave di ordinamento (l'indice della colonna diventa indice della riga quando si ordina da sinistra a destra)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // Definisci l'area di ordinamento (le righe diventano colonne quando si ordina da sinistra a destra)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Esegui l'ordinamento
            sorter.Sort(worksheet.Cells, area);

            // Salva il risultato
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


