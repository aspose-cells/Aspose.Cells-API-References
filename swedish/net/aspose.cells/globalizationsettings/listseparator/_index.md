---
title: "GlobalizationSettings.ListSeparator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-egenskapen. Hämtar avgränsaren för listparametrar i funktion ...etc"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/listseparator/
---
## GlobalizationSettings.ListSeparator property

Hämtar separatorn för lista, funktionsparametrar, ...etc.

```csharp
public virtual char ListSeparator { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Visa aktuellt ListSeparator‑värde från våra anpassade inställningar
            Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);

            // Skapa formel med anpassad listseparator
            worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
            worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";

            // Beräkna formler med anpassad separator
            workbook.CalculateFormula();

            // Visa beräkningsresultat
            Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);

            // Spara med formler med anpassad listseparator
            workbook.Save("ListSeparatorDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ListSeparator => ';';
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


