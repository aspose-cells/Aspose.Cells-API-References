---
title: "CalculationData.CalculatedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationData. Obtiene o establece el valor calculado para esta función"
type: docs
url: /es/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Obtiene o establece el valor calculado para esta función.

```csharp
public object CalculatedValue { get; set; }
```

### Observaciones

El usuario debe establecer esta propiedad en su motor de cálculo personalizado para aquellas funciones que el motor admite, y el valor establecido se devolverá al obtener esta propiedad más tarde. El valor establecido puede ser de tipos posibles de [`Value`](../../cell/value/), o una matriz de ese tipo de valores, o un Range, Name, ReferredArea. Obtener esta propiedad antes de asignarle un valor hará que la función sea calculada por el motor de cálculo predeterminado de Aspose.Cells y luego se devolverá el valor calculado (generalmente debería ser #NAME? para funciones definidas por el usuario).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Crear opciones de cálculo con motor personalizado
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // Calcular fórmulas con opciones
            workbook.CalculateFormula(options);

            // Obtener el valor calculado
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Ver también

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


