---
title: "WorkbookSettings.WindowTopCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret i centimeter"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowtopcm/
---
## WorkbookSettings.WindowTopCM property

Avståndet från övre kanten av klientområdet till övre kanten av fönstret, i enheten centimeter.

```csharp
public double WindowTopCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowTopCMDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in WindowTopCM-egenskapen (position från toppen i centimeter)
            settings.WindowTopCM = 2.5;

            // Visa det aktuella WindowTopCM-värdet
            Console.WriteLine("Window Top Position (cm): " + settings.WindowTopCM);

            // Spara arbetsboken
            workbook.Save("WindowTopCMDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


