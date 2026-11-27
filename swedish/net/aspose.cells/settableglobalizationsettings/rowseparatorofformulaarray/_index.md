---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings egenskap. Hämtar avgränsaren för rader i arraydata i formel"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

Hämtar separatorn för rader i arraydata i formeln.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Visa standardradavgränsaren för formelarrayer
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Ställ in en ny radavgränsare för formelarrayer
            settings.SetRowSeparatorOfFormulaArray(';');

            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            // Skapa en matrisformel i kalkylbladet
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // Beräkna formler
            workbook.CalculateFormula();

            // Spara arbetsboken
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


