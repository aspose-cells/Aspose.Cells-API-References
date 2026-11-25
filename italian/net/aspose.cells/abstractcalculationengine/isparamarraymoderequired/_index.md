---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractCalculationEngine. Indica se questo motore necessita che il parametro sia calcolato in modalità array. Il valore predefinito è false. Se GetParamValueInArrayMode è richiesto durante il calcolo di funzioni personalizzate e l'utente non ha aggiornato la definizione per esse tramite UpdateCustomFunctionDefinition, questa proprietà deve essere impostata su true."
type: docs
url: /it/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Indica se questo motore necessita che il parametro sia calcolato in modalità array. Il valore predefinito è false. Se [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) è richiesto durante il calcolo di funzioni personalizzate e l'utente non ha aggiornato la definizione per esse (tramite [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/)), questa proprietà deve essere impostata su true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Osservazioni

Se questo motore di calcolo personalizzato necessita che il parametro sia calcolato in modalità array, saranno necessari più stack per memorizzare nella cache l'albero dei parametri e il metodo Calculate() potrebbe essere chiamato ricorsivamente per calcolare il valore del parametro. Per motivi di prestazioni, si prega di mantenere questa proprietà al valore predefinito (false) se non vi sono requisiti particolari.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamArrayModeRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomCalculationEngine engine = new CustomCalculationEngine();
            Console.WriteLine("IsParamArrayModeRequired: " + engine.IsParamArrayModeRequired);

            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].Formula = "=SUMARRAY(A1,A2)";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            Console.WriteLine("SUMARRAY result: " + worksheet.Cells["A3"].Value);

            workbook.Save("IsParamArrayModeRequiredDemo.xlsx");
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override bool IsParamArrayModeRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUMARRAY")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(i);

                    double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));

                    sum += param1;
                }
                data.CalculatedValue = sum;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            return false;
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


