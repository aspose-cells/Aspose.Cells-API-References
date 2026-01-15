---
title: AbstractCalculationEngine.IsParamLiteralRequired
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationEngine property. Indicates whether this engine needs the literal text of the parameter while doing a calculation. Default value is false
type: docs
url: /net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Indicates whether this engine needs the literal text of the parameter while doing a calculation. Default value is false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Remarks

If this custom calculation engine needs the parameter's literal text, more stacks will be required to cache the literal text for parameters and Calculate() method may be called recursively to calculate the parameter's value. Generally the literal text is not needed for calculating formulas and this property should be kept as false for most implementations to get better performance.

### Examples

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

            // Create custom calculation engine instance
            MyCustomEngine engine = new MyCustomEngine();

            // Read current property value
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Create test formula with string literal parameter
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Calculate workbook with custom calculation options
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Show calculation result based on property value
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

### See Also

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


