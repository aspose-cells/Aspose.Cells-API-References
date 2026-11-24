---
title: "PageSetup.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Kopiert die Einstellungen der Seiteneinrichtung"
type: docs
url: /de/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Kopiert die Einstellung der Seiteneinrichtung.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | PageSetup | Die Quelle. |
| copyOptions | CopyOptions | Die Kopieroptionen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // PageSetup-Eigenschaften für das erste Arbeitsblatt festlegen
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // PageSetup vom ersten Arbeitsblatt auf das zweite Arbeitsblatt mit CopyOptions kopieren
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### Siehe auch

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


