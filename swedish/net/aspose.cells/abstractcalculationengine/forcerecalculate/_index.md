---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationEngine-metod. Om den angivna funktionen ska tvingas att alltid beräknas om när delade formler beräknas."
type: docs
url: /sv/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

Om den angivna funktionen ska tvingas att alltid beräknas om vid beräkning av delade formler.

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionName | String | namnet på funktionen. Vanligtvis är det det anpassade funktionens namn. Om [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) är sant, kommer inbyggda funktioner också att kontrolleras här. |

### Returvärde

sant om den angivna funktionen alltid behöver beräknas om.

### Anmärkningar

För delade formler delar flera celler samma funktion. Om funktionens parametrar är desamma för dessa celler också, behöver funktionen vanligtvis bara beräknas en gång. Så av prestandaskäl beräknar vi sådan typ av funktion bara en gång också ([`Calculate`](../calculate/) anropas endast en gång, istället för att anropas upprepade gånger för varje cell). Dock, i användarens anpassade implementation kan funktionen, särskilt den anpassade funktionen, behöva beräknas olika för olika celler. I så fall måste användaren åsidosätta denna metod så att den returnerar true för funktionen. Och för [`Calculate`](../calculate/) kan det angivna [`CalculatedValue`](../../calculationdata/calculatedvalue/) ha initierats med det cachade värdet från föregående beräkning.

### Exempel

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

### Se även

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


