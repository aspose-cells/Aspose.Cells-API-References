---
title: "WorkbookSettings.SheetTabBarWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Bredden på kalkylbladsflikfältet i 1/1000 av fönsterbredden"
type: docs
url: /sv/net/aspose.cells/workbooksettings/sheettabbarwidth/
---
## WorkbookSettings.SheetTabBarWidth property

Bredd på arbetsbladets flikrad (i 1/1000 av fönsterbredden).

```csharp
public int SheetTabBarWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySheetTabBarWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in SheetTabBarWidth-egenskapen
            workbook.Settings.SheetTabBarWidth = 1000;
            
            // Hämta och visa SheetTabBarWidth-värdet
            Console.WriteLine("SheetTabBarWidth: " + workbook.Settings.SheetTabBarWidth);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


