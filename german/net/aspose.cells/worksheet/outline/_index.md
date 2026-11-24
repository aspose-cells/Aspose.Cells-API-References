---
title: "Worksheet.Outline"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Gliederung dieses Arbeitsblatts zurück"
type: docs
url: /de/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Ruft die Gliederung dieses Arbeitsblatts ab.

```csharp
public Outline Outline { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten hinzufügen und Gliederungsgruppen erstellen
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // Zeilen gruppieren (erstellt Gliederung)
            worksheet.Cells.GroupRows(0, 9, false);

            // Auf Gliederungseigenschaften zugreifen
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // Gliederungseinstellungen ändern
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // Gruppierung von Zeilen aufheben, um die Gliederungsfunktion zu demonstrieren
            worksheet.Cells.UngroupRows(0, 9);

            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


