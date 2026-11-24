---
title: "WorkbookSettings.ProtectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Ruft den Schutztyp der Arbeitsmappe ab"
type: docs
url: /de/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Liest den Schutztyp der Arbeitsmappe.

```csharp
public ProtectionType ProtectionType { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Schütze die Arbeitsmappe mit dem Windows-Schutztyp
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // Demonstriere die ProtectionType-Eigenschaft
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // Lade die gespeicherte Arbeitsmappe, um zu überprüfen, dass der Schutztyp erhalten bleibt
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### Siehe auch

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


