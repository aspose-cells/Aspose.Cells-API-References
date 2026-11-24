---
title: "Worksheet.ViewType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt den Ansichtstyp zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Ruft den Ansichtstyp ab und setzt ihn.

```csharp
public ViewType ViewType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie den Ansichtstyp auf PageLayoutView und aktivieren Sie das Lineal
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // Fügen Sie Beispielinhalt hinzu, um die Ansicht zu demonstrieren
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### Siehe auch

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


