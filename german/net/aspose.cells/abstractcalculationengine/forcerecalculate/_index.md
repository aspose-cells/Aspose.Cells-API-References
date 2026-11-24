---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationEngine-Methode. Gibt an, ob die gegebene Funktion bei der Berechnung gemeinsamer Formeln immer neu berechnet werden soll."
type: docs
url: /de/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Ob die gegebene Funktion beim Berechnen gemeinsamer Formeln immer neu berechnet werden soll.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionName | String | Name der Funktion. In der Regel ist es der Name einer benutzerdefinierten Funktion. Wenn [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) true ist, werden hier auch integrierte Funktionen überprüft. |

### Rückgabewert

true, wenn die angegebene Funktion immer neu berechnet werden muss.

### Hinweise

Bei gemeinsamen Formeln teilen sich mehrere Zellen dieselbe Funktion. Wenn die Parameter der Funktion für diese Zellen ebenfalls gleich bleiben, muss die Funktion in der Regel nur einmal berechnet werden. Aus Leistungsgründen berechnen wir solche Funktionen daher ebenfalls nur einmal ([`Calculate`](../calculate/) wird nur einmal aufgerufen, anstatt für jede Zelle wiederholt aufzurufen). Bei einer benutzerdefinierten Implementierung kann es jedoch sein, dass die Funktion, insbesondere die benutzerdefinierte Funktion, für verschiedene Zellen unterschiedlich berechnet werden muss. In diesem Fall muss der Benutzer diese Methode überschreiben, damit sie für die Funktion true zurückgibt. Und für [`Calculate`](../calculate/) kann der übergebene [`CalculatedValue`](../../calculationdata/calculatedvalue/) bereits mit dem zwischengespeicherten Wert der vorherigen Berechnung initialisiert sein.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


