---
title: "DeleteBlankOptions.MergedCellsShrinkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DeleteBlankOptions-Eigenschaft. Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden"
type: docs
url: /de/net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Gibt an, wie zusammengeführte Zellen beim Löschen leerer Zeilen/Spalten verarbeitet werden.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Hinweise

Für KeepHeaderOnly werden alle Zellen darin als leer betrachtet, außer der nicht‑leeren oberen linken Zelle. Dies ist der Standardwert dieser Eigenschaft. Für None werden alle Zellen darin als nicht leer betrachtet. Für ShrinkToFit werden alle Zellen außerhalb des Inhaltsanzeigebereichs als leer betrachtet.

### Beispiele

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

            // Beispieldaten mit zusammengeführten Zellen einrichten
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");
            
            // Löschoptionen mit verschiedenen Schrumpfungstypen erstellen
            DeleteBlankOptions options = new DeleteBlankOptions();
            
            // Fall 1: KeepHeaderOnly
            options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Arbeitsblatt zurücksetzen
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Fall 2: ShrinkToFit
            options.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After ShrinkToFit - Merged area adjusted: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Arbeitsblatt zurücksetzen
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Fall 3: None
            options.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After None - Merged area unchanged: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
        }
    }
}
```

### Siehe auch

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


