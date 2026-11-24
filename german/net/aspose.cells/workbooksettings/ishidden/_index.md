---
title: "WorkbookSettings.IsHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob diese Arbeitsmappe ausgeblendet ist"
type: docs
url: /de/net/aspose.cells/workbooksettings/ishidden/
---
## WorkbookSettings.IsHidden property

Gibt an, ob dieses Workbook ausgeblendet ist.

```csharp
public bool IsHidden { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Setze die IsHidden-Eigenschaft auf true
            settings.IsHidden = true;
            Console.WriteLine("Workbook is hidden: " + settings.IsHidden);

            // Speichere die Arbeitsmappe
            workbook.Save("WorkbookSettings_IsHidden_True.xlsx");

            // Erstelle eine weitere Arbeitsmappe
            Workbook workbook2 = new Workbook();

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings2 = workbook2.Settings;

            // Setze die IsHidden-Eigenschaft auf false (Standard)
            settings2.IsHidden = false;
            Console.WriteLine("Workbook is hidden: " + settings2.IsHidden);

            // Speichere die Arbeitsmappe
            workbook2.Save("WorkbookSettings_IsHidden_False.xlsx");

            // Lade und prüfe die gespeicherten Arbeitsmappen
            Workbook loadedWorkbook1 = new Workbook("WorkbookSettings_IsHidden_True.xlsx");
            Console.WriteLine("Loaded workbook1 is hidden: " + loadedWorkbook1.Settings.IsHidden);

            Workbook loadedWorkbook2 = new Workbook("WorkbookSettings_IsHidden_False.xlsx");
            Console.WriteLine("Loaded workbook2 is hidden: " + loadedWorkbook2.Settings.IsHidden);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


