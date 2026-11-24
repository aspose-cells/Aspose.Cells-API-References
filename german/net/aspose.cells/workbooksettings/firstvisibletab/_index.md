---
title: "WorkbookSettings.FirstVisibleTab"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Liest oder setzt das erste sichtbare Arbeitsblatt-Tab"
type: docs
url: /de/net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

Liest oder setzt den ersten sichtbaren Arbeitsblatt-Tab.

```csharp
public int FirstVisibleTab { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFirstVisibleTabDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Einige Arbeitsblätter hinzufügen
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Setzen Sie den Index des ersten sichtbaren Tabs (0‑basiert)
            workbook.Settings.FirstVisibleTab = 1;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Überprüfen Sie die Einstellung
            Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


