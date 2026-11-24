---
title: "Protection.AllowInsertingRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Protection-Eigenschaft. Gibt an, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist."
type: docs
url: /de/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Stellt dar, ob das Einfügen von Zeilen in einem geschützten Arbeitsblatt erlaubt ist

```csharp
public bool AllowInsertingRow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Schutz-Einstellungen
            Protection protection = worksheet.Protection;

            // Einfügen von Zeilen im geschützten Zustand aktivieren
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Versuchen Sie, eine Zeile einzufügen (sollte funktionieren, da AllowInsertingRow true ist)
            worksheet.Cells.InsertRow(0);

            // Speichere die Arbeitsmappe
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


