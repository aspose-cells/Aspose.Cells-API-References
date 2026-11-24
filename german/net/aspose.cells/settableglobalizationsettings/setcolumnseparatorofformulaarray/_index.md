---
title: "SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Legt das Trennzeichen für die Elemente in Zeilendaten von Arrays in einer Formel fest"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray method

Legt das Trennzeichen für die Elemente in den Zeilendaten eines Arrays in der Formel fest.

```csharp
public void SetColumnSeparatorOfFormulaArray(char c)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | Char | der angegebene Trenner |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetColumnSeparatorOfFormulaArrayWithCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            
            try
            {
                globalizationSettings.SetColumnSeparatorOfFormulaArray('|');
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                worksheet.Cells["A1"].SetArrayFormula("{1|2|3}", 1, 3);
                Console.WriteLine("Column separator for formula arrays set to '|'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetColumnSeparatorOfFormulaArray: {ex.Message}");
            }

            workbook.Save("SetColumnSeparatorOfFormulaArrayWithCharDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


