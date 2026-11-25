---
title: "Class DataSorterKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DataSorterKey. Rappresenta la chiave dell'ordinatore dei dati"
type: docs
url: /it/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

Rappresenta la chiave del DataSorter.

```csharp
public class DataSorterKey
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Ottiene il colore ordinato. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Rappresenta l'ID del tipo di set di icone. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Rappresenta il tipo di set di icone. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Ottiene l'indice della colonna ordinata (posizione assoluta, la colonna A è 0, B è 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Indica l'ordine di ordinamento. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Rappresenta il tipo di ordinamento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // Crea un oggetto workbook e carica un file modello
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio da ordinare
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Istanzia l'oggetto data sorter
            DataSorter sorter = workbook.DataSorter;

            // Aggiungi la chiave per la prima colonna (A) da ordinare in ordine crescente
            sorter.AddKey(0, SortOrder.Ascending);

            // Crea un'area di celle (intervallo) da ordinare
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Esegui l'ordinamento
            sorter.Sort(worksheet.Cells, ca);

            // Salva il file di output
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // Accedi a DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Itera attraverso le chiavi e stampa le loro proprietà
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


