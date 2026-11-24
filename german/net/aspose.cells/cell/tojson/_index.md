---
title: "Cell.ToJson"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Konvertiert die Zelle in JSON-Strukturdaten"
type: docs
url: /de/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

Konvertiere [`Cell`](../) in JSON-Strukturdaten.

```csharp
public string ToJson()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten und -stile festlegen
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // Zelle abrufen und in JSON konvertieren
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // Gib das JSON aus
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


