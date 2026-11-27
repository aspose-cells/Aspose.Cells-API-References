---
title: "AutoFitterOptions.OnlyAuto"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Anger om endast rader vars höjd inte är anpassad ska anpassas"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Anger om endast rader vars höjd inte är anpassad ska anpassas.

```csharp
public bool OnlyAuto { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ och ange OnlyAuto-egenskapen
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // Läs in arbetsbok med autoanpassningsalternativ
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // Demonstrera automatisk anpassning genom att kontrollera kolumnbredd
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // Spara och ladda om för att verifiera beständighet
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


