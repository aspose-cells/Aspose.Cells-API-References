---
title: "Worksheet.IsGridlinesVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true"
type: docs
url: /de/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Liest oder setzt einen Wert, der angibt, ob die Gitternetzlinien sichtbar sind. Standard ist true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die Sichtbarkeit der Gitternetzlinien auf true.
            worksheet.IsGridlinesVisible = true;
            
            // Füge einige Beispieldaten hinzu, um Gitterlinien zu sehen.
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // Spalten automatisch anpassen für bessere Sichtbarkeit
            worksheet.AutoFitColumns();
            
            // Speichere die Arbeitsmappe
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


