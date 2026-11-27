---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-metod. Ställ in typen av utskriftsorientering för hela arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Ange typen av utskriftsorientering för hela arbetsboken.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | Typen av sidorientering |

### Exempel

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
            
            // Ställ in sidorientering till Porträtt för alla kalkylblad
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // Verifiera att orienteringen är korrekt inställd
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### Se även

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


