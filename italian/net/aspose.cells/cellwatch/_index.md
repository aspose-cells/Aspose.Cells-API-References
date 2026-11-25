---
title: "Classe CellWatch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CellWatch. Rappresenta l'elemento Cell Watch nella finestra di monitoraggio"
type: docs
url: /it/net/aspose.cells/cellwatch/
---
## CellWatch class

Rappresenta l'Elemento di Monitoraggio Cella nella 'finestra di monitoraggio'.

```csharp
public class CellWatch
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CellWatch](cellwatch/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Ottiene e imposta il nome della cella. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Ottiene e imposta la colonna della cella. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Ottiene e imposta la riga della cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            // Ottieni il primo foglio di lavoro.
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi l'elemento Cell Watch nella finestra di monitoraggio
            int watchIndex = sheet.CellWatches.Add("B2");

            // Recupera l'oggetto CellWatch
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Impostazione delle proprietà
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Salva la cartella di lavoro
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


