---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractCalculationEngine. Indica se questo motore necessita del testo letterale del parametro durante un calcolo. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Indica se questo motore necessita del testo letterale del parametro durante un calcolo. Il valore predefinito è false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Osservazioni

Se questo motore di calcolo personalizzato necessita del testo letterale del parametro, saranno necessari più stack per memorizzare nella cache il testo letterale dei parametri e il metodo Calculate() potrà essere chiamato ricorsivamente per calcolare il valore del parametro. Generalmente il testo letterale non è necessario per il calcolo delle formule e questa proprietà dovrebbe rimanere false nella maggior parte delle implementazioni per ottenere migliori prestazioni.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamLiteralRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza del motore di calcolo personalizzato
            MyCustomEngine engine = new MyCustomEngine();

            // Leggi il valore corrente della proprietà
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Crea una formula di test con parametro stringa letterale
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Calcola cartella di lavoro con opzioni di calcolo personalizzate
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Mostra il risultato del calcolo basato sul valore della proprietà
            Console.WriteLine("Formula result: " + worksheet.Cells["A1"].StringValue);

            workbook.Save("IsParamLiteralRequiredDemo.xlsx");
        }
    }

    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override bool IsParamLiteralRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
            {
                if (data.ParamCount > 0)
                {                    
                    object paramValue = data.GetParamValue(0);
                    string result = (paramValue is string) ? "Literal received" : "Value received";
                    data.CalculatedValue = result;
                }
            }
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


