---
title: "WorkbookSettings.IsHScrollBarVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar eller anger ett värde som indikerar om det genererade kalkylbladet kommer att innehålla ett horisontellt rullningsfält"
type: docs
url: /sv/net/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings.IsHScrollBarVisible property

Hämtar eller anger ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en horisontell rullningslist.

```csharp
public bool IsHScrollBarVisible { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsHScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;
            
            // Dölj det horisontella rullningsfältet
            settings.IsHScrollBarVisible = false;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with horizontal scroll bar hidden.");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


