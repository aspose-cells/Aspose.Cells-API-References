---
title: "WorkbookSettings.WindowWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Bredden på fönstret i enheten punkt"
type: docs
url: /sv/net/aspose.cells/workbooksettings/windowwidth/
---
## WorkbookSettings.WindowWidth property

Fönstrets bredd, i enheten punkt.

```csharp
public double WindowWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWindowWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Ställ in WindowWidth-egenskapen
            settings.WindowWidth = 800;
            
            // Verifiera WindowWidth-värdet
            Console.WriteLine("Window Width set to: " + settings.WindowWidth);
            
            // Spara arbetsboken
            workbook.Save("WindowWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


