---
title: "PivotTableFormatCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotTableFormatCollection proprietà. Ottiene il formato per indice"
type: docs
url: /it/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

Ottiene il formato per indice.

```csharp
public PivotTableFormat this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");

            // Aggiorna tutte le tabelle pivot
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // Accedi alla prima tabella pivot
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // Dimostra la proprietà Item accedendo al primo PivotFormat
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // Modifica le impostazioni di formato utilizzando la proprietà Item
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // Salva la cartella di lavoro modificata
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


