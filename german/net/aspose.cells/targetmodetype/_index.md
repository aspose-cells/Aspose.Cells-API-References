---
title: "Enum TargetModeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TargetModeType-Enum. Stellt den Typ des Zielmodus dar"
type: docs
url: /de/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

Stellt den Typ des Zielmodus dar.

```csharp
public enum TargetModeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| External | `0` | Externer Link |
| FilePath | `1` | Lokale und vollständige Pfade zu Dateien oder Ordnern. |
| Email | `2` | E‑Mail. |
| CellReference | `3` | Link in Zelle oder benanntem Bereich. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Externen Hyperlink hinzufügen
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Den Hyperlink abrufen und dessen TargetModeType prüfen
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // Den Hyperlink löschen
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


