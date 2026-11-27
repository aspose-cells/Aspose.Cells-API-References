---
title: "WorkbookSettings.WindowHeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Fönstrets höjd i enheten tum"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowheightinch/
---
## WorkbookSettings.WindowHeightInch property

Fönstrets höjd, i enheten tum.

```csharp
public double WindowHeightInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in fönsterhöjden i tum
            settings.WindowHeightInch = 5.5;

            // Visa fönsterhöjden i tum
            Console.WriteLine("Window Height in Inches: " + settings.WindowHeightInch);

            // Spara arbetsboken
            workbook.Save("WindowHeightInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


