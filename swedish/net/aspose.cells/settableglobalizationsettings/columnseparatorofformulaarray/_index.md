---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑egenskapen. Hämtar avgränsaren för objekten i raddata för arrayer i formeln"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

Hämtar separatorn för objekten i arrayens raddata i formeln.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Visa det aktuella värdet för ColumnSeparatorOfFormulaArray
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // Ange ett nytt värde för ColumnSeparatorOfFormulaArray
            settings.SetColumnSeparatorOfFormulaArray(';');

            // Applicera inställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            // Skapa en arrayformel med den anpassade avgränsaren med SetArrayFormula
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // Beräkna formler
            workbook.CalculateFormula();

            // Visa resultatet
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // Spara arbetsboken
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


