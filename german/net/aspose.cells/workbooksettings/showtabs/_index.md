---
title: "WorkbookSettings.ShowTabs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Liest oder setzt einen Wert, ob die Registerkarten der Arbeitsmappe angezeigt werden."
type: docs
url: /de/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

Liest oder setzt einen Wert, ob die Arbeitsmappen‑Registerkarten angezeigt werden.

```csharp
public bool ShowTabs { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Blattregisterkarten ausblenden
            workbook.Settings.ShowTabs = false;
            
            // Speichere die Arbeitsmappe
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // Erstellen Sie eine weitere Arbeitsmappe, um die Registerkarten anzuzeigen
            Workbook workbook2 = new Workbook();
            
            // Stellen Sie sicher, dass die Registerkarten sichtbar sind (Standard ist true)
            workbook2.Settings.ShowTabs = true;
            
            // Speichere die Arbeitsmappe
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


