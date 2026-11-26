---
title: "Cell.Calculate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Calcula la fórmula de la celda"
type: docs
url: /es/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Calcula la fórmula de la celda.

```csharp
public void Calculate(CalculationOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | CalculationOptions | Opciones de cálculo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer una fórmula simple en la celda A1
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // Calcular con opciones predeterminadas
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // Establecer una fórmula de matriz en el rango B1:D1
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // Calcular la fórmula de matriz con opciones
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // Establecer una fórmula más compleja en la celda A2
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // Calcular con opciones
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### Ver también

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


