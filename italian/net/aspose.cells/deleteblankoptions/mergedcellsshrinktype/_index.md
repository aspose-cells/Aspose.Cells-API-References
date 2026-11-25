---
title: "DeleteBlankOptions.MergedCellsShrinkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DeleteBlankOptions. Indica come elaborare le celle unite quando si eliminano righe/colonne vuote"
type: docs
url: /it/net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Indica come elaborare le celle unite quando si eliminano righe/colonne vuote.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Osservazioni

Per KeepHeaderOnly, tutte le celle al suo interno saranno considerate vuote eccetto la cella in alto a sinistra non vuota. È il valore predefinito di questa proprietà. Per None, tutte le celle al suo interno saranno considerate non vuote. Per ShrinkToFit, tutte le celle al di fuori dell'area di visualizzazione del contenuto saranno considerate vuote.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Configura dati di esempio con celle unite
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");
            
            // Crea opzioni di cancellazione con diversi tipi di riduzione
            DeleteBlankOptions options = new DeleteBlankOptions();
            
            // Caso 1: KeepHeaderOnly
            options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Reimposta foglio di lavoro
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Caso 2: ShrinkToFit
            options.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After ShrinkToFit - Merged area adjusted: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Reimposta foglio di lavoro
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Caso 3: None
            options.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After None - Merged area unchanged: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
        }
    }
}
```

### Vedi anche

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


