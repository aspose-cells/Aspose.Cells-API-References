---
title: "CalculationOptions.CalcStackSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. El tamaño de pila para calcular celdas recursivamente. El valor predeterminado es 200"
type: docs
url: /es/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

El tamaño de la pila para calcular celdas de forma recursiva. El valor predeterminado es 200.

```csharp
public int CalcStackSize { get; set; }
```

### Observaciones

Cuando hay una gran cantidad de celdas que deben calcularse recursivamente en el árbol de dependencias, puede producirse una StackOverflowException durante el proceso de cálculo. En ese caso, el usuario debe especificar un valor más pequeño para esta propiedad. Para dicha situación, el usuario debe determinar el valor adecuado para esta propiedad según las fórmulas y datos reales. Sin embargo, un valor demasiado pequeño puede provocar una degradación del rendimiento del cálculo de fórmulas y un valor inferior a 2 hará imposible calcular una fórmula que depende de otra. Por lo tanto, si el valor especificado es inferior a 2, se restablecerá a 2.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalcStackSizeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Configure fórmulas de ejemplo que requieran cálculo de pila
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // Calcular con tamaño de pila personalizado
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### Ver también

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


