---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationEngine-egenskap. Anger om denna motor behöver den bokstavliga texten för parametern vid en beräkning. Standardvärdet är false."
type: docs
url: /sv/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Anger om denna motor behöver den bokstavliga texten för parametern under en beräkning. Standardvärdet är falskt.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Anmärkningar

Om denna anpassade beräkningsmotor behöver parameterns bokstavliga text, kommer fler stackar att krävas för att cachea den bokstavliga texten för parametrar och `Calculate()`-metoden kan anropas rekursivt för att beräkna parametervärdet. Vanligtvis behövs den bokstavliga texten inte för att beräkna formler och denna egenskap bör hållas som false för de flesta implementationer för att få bättre prestanda.

### Exempel

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

            // Skapa en instans av anpassad beräkningsmotor
            MyCustomEngine engine = new MyCustomEngine();

            // Läs aktuellt egenskapsvärde
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Skapa testformel med strängbokstavlig parameter
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Beräkna arbetsbok med anpassade beräkningsalternativ
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Visa beräkningsresultat baserat på egenskapsvärde
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

### Se även

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


