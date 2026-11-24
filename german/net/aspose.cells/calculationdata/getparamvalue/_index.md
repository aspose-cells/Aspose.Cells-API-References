---
title: "CalculationData.GetParamValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData-Methode. Gibt das dargestellte Werteobjekt des Parameters an einem angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Liest das dargestellte Wertobjekt des Parameters an einem angegebenen Index.

```csharp
public object GetParamValue(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des Parameters (0‑basiert) |

### Rückgabewert

Der berechnete Wert des Parameters.

### Hinweise

Für einen Parameter:

Wenn es ein einfacher Wert ist, wird der einfache Wert selbst zurückgegeben;

Wenn es eine Referenz ist, wird das ReferredArea‑Objekt zurückgegeben;

Wenn es sich auf Datensatz(e) mit mehreren Werten bezieht, gibt es ein Array von Objekten zurück;

Wenn es sich um eine Art Ausdruck handelt, der berechnet werden muss, wird er im Werte‑Modus berechnet und in der Regel ein einzelner Wert gemäß der aktuellen Zellenbasis zurückgegeben. Zum Beispiel, wenn ein Parameter der Formel von D2 A:A+B:B ist, wird A2+B2 berechnet und zurückgegeben. Wird dieser Parameter jedoch als Array‑Modus angegeben (über [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) oder [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), wird ein Array (object[][]) zurückgegeben, dessen Elemente A1+B1,A2+B2,....

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://localhost:9090\", \"Target\")";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new HyperlinkCalculationEngine();
            workbook.CalculateFormula(options);
        }

        class HyperlinkCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.Equals("HYPERLINK", StringComparison.OrdinalIgnoreCase))
                {
                    Console.WriteLine("URL Parameter: " + data.GetParamValue(0));
                    Console.WriteLine("Display Text: " + data.GetParamValue(1));
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


