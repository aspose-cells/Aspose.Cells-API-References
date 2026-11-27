---
title: "WorkbookSettings.IsVScrollBarVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar eller anger ett värde som visar om det genererade kalkylbladet kommer att innehålla en vertikal rullningslist"
type: docs
url: /sv/net/aspose.cells/workbooksettings/isvscrollbarvisible/
---
## WorkbookSettings.IsVScrollBarVisible property

Hämtar eller anger ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en vertikal rullningslist.

```csharp
public bool IsVScrollBarVisible { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsVScrollBarVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;
            
            // Dölj den vertikala rullningslisten
            settings.IsVScrollBarVisible = false;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Vertical scroll bar visibility set to false. Workbook saved.");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


