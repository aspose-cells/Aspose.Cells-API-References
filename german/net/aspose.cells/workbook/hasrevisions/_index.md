---
title: "Workbook.HasRevisions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt an, ob die Arbeitsmappe nachverfolgte Änderungen enthält"
type: docs
url: /de/net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Liest, ob die Arbeitsmappe nachverfolgte Änderungen enthält

```csharp
public bool HasRevisions { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasRevisionsDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit Revisionen erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Führe eine Änderung durch, die eine Revision erzeugt
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Prüfe, ob die Arbeitsmappe Revisionen enthält
            Console.WriteLine("Workbook has revisions: " + workbook.HasRevisions);
            
            // Alle Revisionen akzeptieren (falls vorhanden)
            if (workbook.HasRevisions)
            {
                workbook.AcceptAllRevisions();
            }
            
            // Erneut prüfen nach dem Akzeptieren von Revisionen
            Console.WriteLine("Workbook has revisions after accepting: " + workbook.HasRevisions);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


