---
title: "CalculationData.CalculatedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData-Eigenschaft. Liest oder schreibt den berechneten Wert für diese Funktion"
type: docs
url: /de/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Liest oder setzt den berechneten Wert für diese Funktion.

```csharp
public object CalculatedValue { get; set; }
```

### Hinweise

Der Benutzer sollte diese Eigenschaft in seiner benutzerdefinierten Berechnungs‑Engine für die von der Engine unterstützten Funktionen setzen, und der gesetzte Wert wird beim späteren Abrufen dieser Eigenschaft zurückgegeben. Der gesetzte Wert kann mögliche Typen von [`Value`](../../cell/value/), ein Array solcher Werte oder einen Bereich, Namen, ReferredArea sein. Das Abrufen dieser Eigenschaft, bevor ein Wert gesetzt wurde, führt dazu, dass die Funktion von der Standard‑Berechnungs‑Engine von Aspose.Cells berechnet wird und dann der berechnete Wert zurückgegeben wird (in der Regel sollte dies #NAME? für benutzerdefinierte Funktionen sein).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Erstelle Berechnungsoptionen mit benutzerdefinierter Engine
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // Formeln mit Optionen berechnen
            workbook.CalculateFormula(options);

            // Den berechneten Wert abrufen
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
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

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


