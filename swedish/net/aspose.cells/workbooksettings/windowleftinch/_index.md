---
title: "WorkbookSettings.WindowLeftInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten tum"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowleftinch/
---
## WorkbookSettings.WindowLeftInch property

Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten tum.

```csharp
public double WindowLeftInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Ange egenskapen WindowLeftInch
            settings.WindowLeftInch = 1.5; // Position window 1.5 inches from left edge of screen

            // Lägg till lite exempeldata för att demonstrera att arbetsboken fungerar
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Window left position: {settings.WindowLeftInch} inches");

            // Spara arbetsboken
            workbook.Save("WindowLeftInchDemo.xlsx");

            Console.WriteLine("Workbook saved with WindowLeftInch = " + settings.WindowLeftInch);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


