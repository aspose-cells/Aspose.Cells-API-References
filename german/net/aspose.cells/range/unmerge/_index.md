---
title: "Range.UnMerge"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Löst zusammengeführte Zellen dieses Bereichs auf"
type: docs
url: /de/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Löst zusammengeführte Zellen dieses Bereichs.

```csharp
public void UnMerge()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zellen B2 bis D4 zusammenführen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // Überprüfe, ob Zelle B2 vor dem Aufheben der Zusammenführung zusammengeführt ist
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // Löse die Zusammenführung des Bereichs auf
            range.UnMerge();
            
            // Überprüfe, ob Zelle B2 nach dem Aufheben der Zusammenführung zusammengeführt ist
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


