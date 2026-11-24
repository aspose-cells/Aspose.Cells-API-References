---
title: "CalculationData.ParamCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData-Eigenschaft. Gibt die Anzahl der Parameter zurück"
type: docs
url: /de/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Liest die Anzahl der Parameter

```csharp
public int ParamCount { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Füllen Sie einige Zellen, die als Parameter verwendet werden, aus
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Setzen Sie eine Formel, die eine benutzerdefinierte Funktion mit drei Argumenten aufruft
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Konfiguriere die Berechnungsoptionen, um eine benutzerdefinierte Engine zu verwenden
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Berechnung durchführen
                workbook.CalculateFormula(options);

                // Die benutzerdefinierte Engine gibt ParamCount als berechneten Wert zurück
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // Optional das Arbeitsbuch speichern
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Benutzerdefinierte Berechnungs‑Engine, die das Lesen der ParamCount‑Eigenschaft demonstriert
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Identifizieren Sie die benutzerdefinierte Funktion anhand ihres Namens
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Lesen Sie die schreibgeschützte ParamCount‑Eigenschaft
                    int count = data.ParamCount;

                    // Verwenden Sie die Anzahl als Ergebnis der Funktion
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### Siehe auch

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


