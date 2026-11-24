---
title: "Outline.SummaryColumnRight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Outline-Eigenschaft. Gibt an, ob die Zusammenfassungsspalte rechts von den Detailspalten in der Gliederung positioniert wird"
type: docs
url: /de/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Gibt an, ob die Zusammenfassungsspalte rechts von den Detailspalten in der Gliederung positioniert wird.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten hinzufügen und Zeilen gruppieren
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Zeilen gruppieren (erstellt eine Gliederung)
            worksheet.Cells.GroupRows(0, 9, false);

            // Gliederungseinstellungen abrufen
            Outline outline = worksheet.Outline;

            // SummaryColumnRight auf true setzen (Zusammenfassungsspalten erscheinen rechts von den Detailspalten)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // Speichere die Arbeitsmappe
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


