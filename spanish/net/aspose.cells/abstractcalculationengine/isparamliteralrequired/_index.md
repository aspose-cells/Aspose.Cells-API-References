---
title: "AbstractCalculationEngine.IsParamLiteralRequired"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de AbstractCalculationEngine. Indica si este motor necesita el texto literal del parámetro al realizar un cálculo. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/abstractcalculationengine/isparamliteralrequired/
---
## AbstractCalculationEngine.IsParamLiteralRequired property

Indica si este motor necesita el texto literal del parámetro durante un cálculo. El valor predeterminado es false.

```csharp
public virtual bool IsParamLiteralRequired { get; }
```

### Observaciones

Si este motor de cálculo personalizado necesita el texto literal del parámetro, se requerirán más pilas para almacenar en caché el texto literal de los parámetros y el método Calculate() puede llamarse recursivamente para calcular el valor del parámetro. Generalmente, el texto literal no es necesario para calcular fórmulas y esta propiedad debería mantenerse como false en la mayoría de las implementaciones para obtener mejor rendimiento.

### Ejemplos

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

            // Crear una instancia del motor de cálculo personalizado
            MyCustomEngine engine = new MyCustomEngine();

            // Leer el valor actual de la propiedad
            Console.WriteLine("Current IsParamLiteralRequired value: " + engine.IsParamLiteralRequired);

            // Crear una fórmula de prueba con un parámetro literal de cadena
            worksheet.Cells["A1"].Formula = "=MYFUNC(\"123\")";

            // Calcular libro de trabajo con opciones de cálculo personalizadas
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            // Mostrar el resultado del cálculo basado en el valor de la propiedad
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

### Ver también

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


