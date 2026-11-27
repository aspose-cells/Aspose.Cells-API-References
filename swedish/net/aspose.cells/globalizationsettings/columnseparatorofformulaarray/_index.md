---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-egenskap. Hämtar avgränsaren för objekten i rader med arraydata i formeln"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

Hämtar separatorn för objekten i arrayens raddata i formeln.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar med överskriven kolumnavgränsare
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Visa aktuellt värde för kolumnavgränsare
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // Skapa arrayformel med anpassad avgränsare
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // Verifiera formellagring (skulle visa semikolon i den faktiska formelsträngen)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // Spara modifierad arbetsbok
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


