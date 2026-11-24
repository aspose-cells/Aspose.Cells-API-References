---
title: "Row.GroupLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt die Gruppenebene der Zeile zurück"
type: docs
url: /de/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Gibt die Gruppierungsebene der Zeile zurück.

```csharp
public byte GroupLevel { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruppiere Zeilen 4-6 (hidden = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // Greifen Sie auf die Gruppenebene von Zeile 4 zu
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // Gruppierung der Zeilen aufheben
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


