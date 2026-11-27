---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar alternativen för smart-taggen"
type: docs
url: /sv/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Hämtar alternativen för smart-taggen.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();

                // Kom åt arbetsbokens inställningar
                WorkbookSettings settings = workbook.Settings;

                // Läs SmartTagOptions-egenskapen
                var smartTagOptions = settings.SmartTagOptions;

                // Visa information om SmartTagOptions-instansen
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // Eventuellt kan du inspektera standardtillståndet via ToString()
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Spara arbetsboken (filen kommer att innehålla standardinställningar)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


