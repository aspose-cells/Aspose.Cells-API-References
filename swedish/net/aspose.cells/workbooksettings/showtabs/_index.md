---
title: "WorkbookSettings.ShowTabs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Hämtar eller anger ett värde för om arbetsbokens flikar visas"
type: docs
url: /sv/net/aspose.cells/workbooksettings/showtabs/
---
## WorkbookSettings.ShowTabs property

Hämtar eller anger ett värde om arbetsbokens flikar visas.

```csharp
public bool ShowTabs { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyShowTabsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Dölj kalkylbladsflikarna
            workbook.Settings.ShowTabs = false;
            
            // Spara arbetsboken
            workbook.Save("HideTabsDemo.xlsx", SaveFormat.Xlsx);
            
            // Skapa en annan arbetsbok för att visa flikar
            Workbook workbook2 = new Workbook();
            
            // Säkerställ att flikarna är synliga (standard är sant)
            workbook2.Settings.ShowTabs = true;
            
            // Spara arbetsboken
            workbook2.Save("ShowTabsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


