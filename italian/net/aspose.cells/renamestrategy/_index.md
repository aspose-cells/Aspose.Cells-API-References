---
title: "Enum RenameStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.RenameStrategy enum. Opzione di strategia per nomi duplicati delle colonne."
type: docs
url: /it/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Opzione di strategia per nomi duplicati delle colonne.

```csharp
public enum RenameStrategy
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Exception | `0` | Lancia un'eccezione. |
| Digit | `1` | Denominato con cifra. I nomi duplicati diventeranno ...1, ...2, ecc. |
| Letter | `2` | Denominato con lettera. I nomi duplicati diventeranno ...A, ...B, ecc. |

### Osservazioni

Durante l'elaborazione dei dati con intestazioni, alcuni scenari richiedono che le intestazioni non siano duplicate per tutte le colonne. Ad esempio, quando si esportano i dati in un DataTable e l'intestazione deve essere utilizzata come nome della colonna del DataTable, i valori duplicati dell'intestazione sono invalidi. Per questo tipo di situazioni, l'utente può determinare come gestirle specificando questa strategia.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // Crea ExportTableOptions e imposta RenameStrategy.
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Esporta i dati del foglio di lavoro in un DataTable.
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // Visualizza il contenuto del DataTable.
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Salva la cartella di lavoro
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


