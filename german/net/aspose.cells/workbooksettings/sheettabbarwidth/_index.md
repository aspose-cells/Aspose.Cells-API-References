---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Breite der Arbeitsblatt-Tab-Leiste in 1/1000 der Fensterbreite."
type: docs
url: /de/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Breite der Arbeitsblatt‑Registerkartenleiste (in 1/1000 der Fensterbreite).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setzen Sie die SheetTabBarWidth-Eigenschaft.
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // Abrufen und Anzeigen des SheetTabBarWidth-Werts.
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


