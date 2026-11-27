---
title: "WorkbookSettings.WindowLeft"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret i enheten punkt"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowleft/
---
## WorkbookSettings.WindowLeft property

Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret, i enheten punkt.

```csharp
public double WindowLeft { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowLeftDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Ställ in WindowLeft-egenskapen för att placera fönstret 100 pixlar från vänster
            settings.WindowLeft = 100;

            // Ställ in andra fönsteregenskaper för demonstration
            settings.WindowTop = 50;
            settings.WindowWidth = 800;
            settings.WindowHeight = 600;

            // Lägg till exempeldata i arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Window Position Demo");
            sheet.Cells["A2"].PutValue($"Left: {settings.WindowLeft}px");
            sheet.Cells["A3"].PutValue($"Top: {settings.WindowTop}px");

            // Spara arbetsboken
            workbook.Save("WindowPositionDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


