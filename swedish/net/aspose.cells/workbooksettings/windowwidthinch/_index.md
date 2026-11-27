---
title: "WorkbookSettings.WindowWidthInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Bredden på fönstret i enheten tum"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowwidthinch/
---
## WorkbookSettings.WindowWidthInch property

Fönstrets bredd, i enheten tum.

```csharp
public double WindowWidthInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in fönsterbredd i tum
            settings.WindowWidthInch = 10.5;

            // Visa fönsterbredden i tum
            Console.WriteLine("Window Width in Inches: " + settings.WindowWidthInch);

            // Spara arbetsboken
            workbook.Save("WindowWidthInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


