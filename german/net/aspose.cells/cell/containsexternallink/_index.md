---
title: "Cell.ContainsExternalLink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle ein Formelfeld ist."
type: docs
url: /de/net/aspose.cells/cell/containsexternallink/
---
## Cell.ContainsExternalLink property

Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist.

```csharp
public bool ContainsExternalLink { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyContainsExternalLinkDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];
            
            // Beispieldaten und externen Link hinzufügen
            sheet.Cells["A1"].PutValue("External Link:");
            sheet.Cells["B1"].Formula = "=HYPERLINK(\"https://www.aspose.com\", \"Aspose\")";
            
            // Prüfen, ob Zellen externe Links enthalten
            Console.WriteLine("A1 ContainsExternalLink: " + sheet.Cells["A1"].ContainsExternalLink);
            Console.WriteLine("B1 ContainsExternalLink: " + sheet.Cells["B1"].ContainsExternalLink);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


