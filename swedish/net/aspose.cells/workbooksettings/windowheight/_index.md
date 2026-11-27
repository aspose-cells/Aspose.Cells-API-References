---
title: "WorkbookSettings.WindowHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Fönstrets höjd i enheten punkt"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowheight/
---
## WorkbookSettings.WindowHeight property

Fönstrets höjd, i enheten punkt.

```csharp
public double WindowHeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Sätt WindowHeight-egenskapen
            settings.WindowHeight = 600;
            
            // Verifiera WindowHeight-värdet
            Console.WriteLine("Window Height set to: " + settings.WindowHeight);
            
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


