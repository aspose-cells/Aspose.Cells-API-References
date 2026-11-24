---
title: "Style.IsJustifyDistributed"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob für die letzte Zeile des Textes die Block‑ oder Verteilt‑Ausrichtung verwendet werden soll"
type: docs
url: /de/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Gibt an, ob die Zellen im Block- oder verteilten Ausrichtungsmodus in der letzten Textzeile verwendet werden sollen.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Hinweise

Dies ist typisch für ostasiatische Ausrichtungen, aber nicht in anderen Kontexten. Funktioniert nur bei verteilter horizontaler Ausrichtung.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf Zelle B3 zu und setzen Sie deren Text
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // Rufen Sie den Stil der Zelle ab und setzen Sie IsJustifyDistributed auf true
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Überprüfen Sie die Eigenschaft
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


