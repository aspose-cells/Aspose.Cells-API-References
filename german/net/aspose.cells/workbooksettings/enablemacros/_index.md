---
title: "WorkbookSettings.EnableMacros"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Aktiviert Makros"
type: docs
url: /de/net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Makros aktivieren;

```csharp
public bool EnableMacros { get; set; }
```

### Hinweise

Jetzt funktioniert es nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt in einer Arbeitsmappe.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // Demonstriere die EnableMacros-Eigenschaft
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // Makros deaktivieren
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // Makros aktivieren
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // Speichere die Arbeitsmappe
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


