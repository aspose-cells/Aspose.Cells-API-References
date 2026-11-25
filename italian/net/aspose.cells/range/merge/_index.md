---
title: "Range.Merge"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Combina un intervallo di celle in un'unica cella"
type: docs
url: /it/net/aspose.cells/range/merge/
---
## Range.Merge method

Combina un intervallo di celle in una singola cella.

```csharp
public void Merge()
```

### Osservazioni

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo e unisci le celle (3 righe x 2 colonne)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // Imposta il valore nella cella unita
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // Applica lo stile alle celle unite
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


