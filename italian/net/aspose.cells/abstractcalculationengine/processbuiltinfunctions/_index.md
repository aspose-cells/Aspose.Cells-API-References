---
title: "AbstractCalculationEngine.ProcessBuiltInFunctions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractCalculationEngine. Indica se le funzioni builtin supportate dal motore builtin devono essere verificate e elaborate da questa implementazione. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/abstractcalculationengine/processbuiltinfunctions/
---
## AbstractCalculationEngine.ProcessBuiltInFunctions property

Indica se le funzioni integrate supportate dal motore integrato debbano essere verificate ed elaborate da questa implementazione. Il valore predefinito è false.

```csharp
public virtual bool ProcessBuiltInFunctions { get; }
```

### Osservazioni

Se l'utente deve modificare la logica di calcolo di alcune funzioni built-in, questa proprietà deve essere impostata su true. Altrimenti, si prega di lasciare questa proprietà su false per motivi di prestazioni.

### Esempi

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
            
            // Popola dati di test
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Crea motori di calcolo personalizzati con valori diversi di ProcessBuiltInFunctions
            CustomEngine engineProcessEnabled = new CustomEngine(true);
            CustomEngine engineProcessDisabled = new CustomEngine(false);

            // Mostra i valori delle proprietà
            Console.WriteLine("Engine1 ProcessBuiltInFunctions: " + engineProcessEnabled.ProcessBuiltInFunctions);
            Console.WriteLine("Engine2 ProcessBuiltInFunctions: " + engineProcessDisabled.ProcessBuiltInFunctions);

            // Calcola con motore personalizzato (ProcessBuiltInFunctions = true)
            CalculationOptions optionsEnabled = new CalculationOptions { CustomEngine = engineProcessEnabled };
            workbook.CalculateFormula(optionsEnabled);
            Console.WriteLine("Result with ProcessBuiltInFunctions=true: " + worksheet.Cells["A4"].Value);

            // Calcola con motore personalizzato (ProcessBuiltInFunctions = false)
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
            // Altre funzioni sono gestite dal motore predefinito
        }

        public override bool ForceRecalculate(string functionName) => false;
    }
}
```

### Vedi anche

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


