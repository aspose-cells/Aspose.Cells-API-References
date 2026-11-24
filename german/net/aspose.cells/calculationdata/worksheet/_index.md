---
title: "CalculationData.Worksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData-Eigenschaft. Gibt das Worksheet-Objekt zurück, in dem die Funktion ist"
type: docs
url: /de/net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Liest das Worksheet-Objekt, in dem sich die Funktion befindet.

```csharp
public Worksheet Worksheet { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Erstelle Berechnungsoptionen mit benutzerdefinierter Engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // Formeln mit Optionen berechnen
                workbook.CalculateFormula(options);

                // Ergebnis anzeigen
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Ergebnis speichern
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Greife auf die schreibgeschützte Worksheet-Eigenschaft zu
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


