---
title: "CalculationCell.SetCalculatedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationCell-Methode. Setzt den berechneten Wert für die Zelle"
type: docs
url: /de/net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Setzt den berechneten Wert für die Zelle.

```csharp
public void SetCalculatedValue(object v)
```

### Hinweise

Der Benutzer kann das berechnete Ergebnis mit dieser Methode festlegen, um die automatische Berechnung für die Zelle zu ignorieren.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Erstelle eine CalculationCell-Instanz mittels Reflexion, da der Konstruktor nicht öffentlich ist.
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Setzen Sie einen berechneten Wert mithilfe der SetCalculatedValue-Methode
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Zeigen Sie Informationen über die Zelle an
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Speichere die Arbeitsmappe
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


