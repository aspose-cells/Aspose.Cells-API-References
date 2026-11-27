---
title: "WorkbookSettings.WindowHeightCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Fönstrets höjd i enheten centimeter"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowheightcm/
---
## WorkbookSettings.WindowHeightCM property

Fönstrets höjd, i enheten centimeter.

```csharp
public double WindowHeightCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightCMDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in WindowHeightCM-egenskapen
            settings.WindowHeightCM = 15.5;

            // Visa det angivna värdet
            Console.WriteLine("Window Height in Centimeters: " + settings.WindowHeightCM);

            // Spara arbetsboken
            workbook.Save("WindowHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


