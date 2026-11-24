---
title: "Style.IsDateTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob das Zahlenformat ein Datumsformat ist"
type: docs
url: /de/net/aspose.cells/style/isdatetime/
---
## Style.IsDateTime property

Gibt an, ob das Zahlenformat ein Datumsformat ist.

```csharp
public bool IsDateTime { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsDateTimeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Setze einen numerischen Wert
            cells["A1"].PutValue(1230);
            
            // Lese und ändere den Stil der Zelle
            Style style = cells["A1"].GetStyle();
            
            // Setze auf Datumsformat (15 ist das integrierte Datumsformat)
            style.Number = 15;
            Console.WriteLine("IsDateTime after setting Number=15: " + style.IsDateTime);
            
            // Setze benutzerdefiniertes Datumsformat
            style.Custom = "yyyy-mm-dd";
            Console.WriteLine("IsDateTime after setting custom date format: " + style.IsDateTime);
            
            // Wende den modifizierten Stil wieder auf die Zelle an
            cells["A1"].SetStyle(style);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


