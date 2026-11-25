---
title: "Cells.TextToColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Divide il contenuto nella colonna specificata in più colonne"
type: docs
url: /it/net/aspose.cells/cells/texttocolumns/
---
## Cells.TextToColumns method

Divide il contenuto nella colonna specificata in più colonne..

```csharp
public int TextToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |
| totalRows | Int32 | Il numero di righe. |
| opzioni | TxtLoadOptions | Le opzioni di divisione. |

### Valore di ritorno

Numero totale di colonne dei valori divisi.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodTextToColumnsWithInt32Int32Int32TxtLoadOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta dati di esempio con valori separati da virgola
            sheet.Cells["A1"].PutValue("John,Doe,30");
            sheet.Cells["A2"].PutValue("Jane,Smith,28");

            // Crea opzioni di caricamento testo con la virgola come separatore
            TxtLoadOptions options = new TxtLoadOptions();
            options.Separator = ',';

            // Dividi il testo in colonne a partire dalla cella A1, larga 3 colonne
            sheet.Cells.TextToColumns(0, 0, 3, options);

            // Verifica i risultati
            Console.WriteLine("B1: " + sheet.Cells["B1"].StringValue); // Should output "Doe"
            Console.WriteLine("C2: " + sheet.Cells["C2"].StringValue); // Should output "28"

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


