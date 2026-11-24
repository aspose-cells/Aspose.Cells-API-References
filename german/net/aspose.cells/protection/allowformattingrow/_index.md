---
title: "Protection.AllowFormattingRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob das Formatieren von Zeilen in einem geschützten Arbeitsblatt erlaubt ist."
type: docs
url: /de/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

Stellt dar, ob das Formatieren von Zeilen in einem geschützten Arbeitsblatt erlaubt ist

```csharp
public bool AllowFormattingRow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arbeitsblattschutz aktivieren
            worksheet.Protect(ProtectionType.All);

            // Auf Schutz-Einstellungen zugreifen
            Protection protection = worksheet.Protection;

            // Erlaube das Formatieren von Zeilen, während andere Schutzmaßnahmen beibehalten werden.
            protection.AllowFormattingRow = true;

            // Speichere die Arbeitsmappe
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


