---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationData‑Methode. Gibt die Werte des Parameters an einem angegebenen Index zurück. Wenn der Parameter eine Art Ausdruck ist, der berechnet werden muss, wird er im Array‑Modus berechnet."
type: docs
url: /de/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Liest den/die Wert(e) des Parameters an einem angegebenen Index. Wenn der Parameter eine Art Ausdruck ist, der berechnet werden muss, wird er im Array-Modus berechnet.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index des Parameters (0‑basiert) |
| maxRowCount | Int32 | Die Zeilenanzahlbegrenzung für das zurückgegebene Array. Ist sie nicht positiv oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Zeilenanzahl verwendet. |
| maxColumnCount | Int32 | Die Spaltenanzahlbegrenzung für das zurückgegebene Array. Ist sie nicht positiv oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Spaltenanzahl verwendet. |

### Rückgabewert

Ein Array, das alle durch den angegebenen Parameter dargestellten Elemente enthält.

### Hinweise

Für einen Ausdruck, der berechnet werden muss, am Beispiel A:A+B:B: Im Werte‑Modus wird er zu einem einzelnen Wert gemäß der aktuellen Zellenbasis berechnet. Im Array‑Modus werden jedoch alle Werte von A1+B1, A2+B2, A3+B3, … berechnet und zum Erstellen des zurückgegebenen Arrays verwendet. Für solche Situationen ist es besser, die Begrenzung für die Zeilen‑/Spaltenanzahl anzugeben (z. B. gemäß [`MaxDataRow`](../../cells/maxdatarow/) und [`MaxDataColumn`](../../cells/maxdatacolumn/)), da sonst das zurückgegebene große Array mit vielen unnützen Daten den Speicherverbrauch erhöhen kann.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Kontext hinzufügen
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Erstelle Berechnungsoptionen mit benutzerdefinierter Engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Rufen Sie GetParamValueInArrayMode mit realistischen Parametern auf
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
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


