---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Methode. Legen Sie den Typ der Druckausrichtung für die gesamte Arbeitsmappe fest"
type: docs
url: /de/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Legt den Typ der Druckausrichtung für die gesamte Arbeitsmappe fest.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | Der Typ der Seitenorientierung |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            
            // Setzen Sie die Seitenorientierung für alle Arbeitsblätter auf Hochformat
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // Überprüfen Sie, ob die Orientierung korrekt eingestellt ist
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### Siehe auch

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


