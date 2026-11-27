---
title: "AbstractCalculationEngine.ProcessBuiltInFunctions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationEngine egenskap. Huruvida inbyggda funktioner som har stöd av den inbyggda motorn ska kontrolleras och bearbetas av denna implementation. Standard är falskt."
type: docs
url: /sv/net/aspose.cells/abstractcalculationengine/processbuiltinfunctions/
---
## AbstractCalculationEngine.ProcessBuiltInFunctions property

Om inbyggda funktioner som stöds av den inbyggda motorn ska kontrolleras och bearbetas av denna implementation. Standard är falskt.

```csharp
public virtual bool ProcessBuiltInFunctions { get; }
```

### Anmärkningar

Om användaren behöver ändra beräkningslogiken för vissa inbyggda funktioner, bör denna egenskap sättas till true. Annars vänligen lämna egenskapen som false av prestandaskäl.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyProcessBuiltInFunctionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i testdata
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Skapa anpassade beräkningsmotorer med olika ProcessBuiltInFunctions‑värden
            CustomEngine engineProcessEnabled = new CustomEngine(true);
            CustomEngine engineProcessDisabled = new CustomEngine(false);

            // Visa egenskapsvärden
            Console.WriteLine("Engine1 ProcessBuiltInFunctions: " + engineProcessEnabled.ProcessBuiltInFunctions);
            Console.WriteLine("Engine2 ProcessBuiltInFunctions: " + engineProcessDisabled.ProcessBuiltInFunctions);

            // Beräkna med anpassad motor (ProcessBuiltInFunctions = true)
            CalculationOptions optionsEnabled = new CalculationOptions { CustomEngine = engineProcessEnabled };
            workbook.CalculateFormula(optionsEnabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=true: " + worksheet.Cells["A4"].Value);

            // Beräkna med anpassad motor (ProcessBuiltInFunctions = false)
            CalculationOptions optionsDisabled = new CalculationOptions { CustomEngine = engineProcessDisabled };
            workbook.CalculateFormula(optionsDisabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=false: " + worksheet.Cells["A4"].Value);

            workbook.Save("ProcessBuiltInFunctionsDemo.xlsx");
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        private readonly bool _processBuiltIn;

        public CustomEngine(bool processBuiltIn)
        {
            _processBuiltIn = processBuiltIn;
        }

        public override bool ProcessBuiltInFunctions => _processBuiltIn;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("SUM", StringComparison.OrdinalIgnoreCase) && ProcessBuiltInFunctions)
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object param = data.GetParamValue(i);
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);

                    for (int r = paramArea1.StartRow; r <= paramArea1.EndRow; r++)
                    {
                        for (int c = paramArea1.StartColumn; c <= paramArea1.EndColumn; c++)
                        {
                            object cellValue = paramArea1.GetValue(r, c);
                            sum += Convert.ToDouble(cellValue);
                        }
                    }
                    
                }
                data.CalculatedValue = sum * 2; // Custom SUM implementation doubles the result
            }
            // Andra funktioner hanteras av standardmotorn
        }

        public override bool ForceRecalculate(string functionName) => false;
    }
}
```

### Se även

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


