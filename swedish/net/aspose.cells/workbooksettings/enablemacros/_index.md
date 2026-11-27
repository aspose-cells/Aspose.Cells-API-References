---
title: "WorkbookSettings.EnableMacros"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings egenskap. Aktivera makron"
type: docs
url: /sv/net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Aktivera makron;

```csharp
public bool EnableMacros { get; set; }
```

### Anmärkningar

Nu fungerar det bara när du kopierar ett kalkylblad till ett annat kalkylblad i en arbetsbok.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // Demonstrera egenskapen EnableMacros
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // Inaktivera makron
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // Aktivera makron
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // Spara arbetsboken
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


