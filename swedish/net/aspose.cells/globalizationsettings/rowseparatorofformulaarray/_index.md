---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-egenskapen. Hämtar avgränsaren för rader i arraydata i formeln"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

Hämtar separatorn för rader i arraydata i formeln.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med anpassade globaliseringsinställningar
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till den anpassade GlobalizationSettings-instansen
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // Visa det aktuella värdet för RowSeparatorOfFormulaArray
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Skapa en arrayformel med den anpassade radavgränsaren
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // Beräkna formeln för att demonstrera korrekt parsning
            workbook.CalculateFormula();

            // Visa resultat
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // Spara arbetsboken
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // Anpassad GlobalizationSettings-implementation som åsidosätter radavgränsaren
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


