---
title: "DeleteBlankOptions.MergedCellsShrinkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteBlankOptions egenskap. Anger hur sammanslagna celler ska behandlas när tomma rader/kolumner tas bort"
type: docs
url: /sv/net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Anger hur sammanslagna celler ska behandlas när tomma rader/kolumner tas bort.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Anmärkningar

För KeepHeaderOnly kommer alla celler i den att betraktas som tomma förutom den icke‑tomma övre vänstra cellen. Det är standardvärdet för denna egenskap. För None kommer alla celler i den att betraktas som icke‑tomma. För ShrinkToFit kommer alla celler utanför innehållsområdet att betraktas som tomma.

### Exempel

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

            // Skapa exempeldata med sammanslagna celler
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");
            
            // Skapa raderingsalternativ med olika krympningstyper
            DeleteBlankOptions options = new DeleteBlankOptions();
            
            // Fall 1: KeepHeaderOnly
            options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Återställ kalkylbladet
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

            // Återställ kalkylbladet
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

### Se även

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


