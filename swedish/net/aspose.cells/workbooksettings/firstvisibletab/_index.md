---
title: "WorkbookSettings.FirstVisibleTab"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar eller anger den första synliga kalkylbladsfliken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

Hämtar eller anger den första synliga arbetsbladfliken.

```csharp
public int FirstVisibleTab { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFirstVisibleTabDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några arbetsblad
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Ange index för den första synliga fliken (0‑baserat)
            workbook.Settings.FirstVisibleTab = 1;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Verifiera inställningen
            Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


