---
title: "Cell.GetArrayRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene el rango de matriz si la fórmula de la celda es una fórmula de matriz"
type: docs
url: /es/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Obtiene el rango de matriz si la fórmula de la celda es una fórmula de matriz.

```csharp
public CellArea GetArrayRange()
```

### Valor de retorno

El rango de matriz.

### Observaciones

Solo se aplica cuando la fórmula de la celda es una fórmula de matriz

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Establezca una fórmula de matriz dinámica en la celda A1
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // Calcular fórmulas
            wb.CalculateFormula();
            
            // Obtener el rango de matriz de la fórmula dinámica
            CellArea arrayRange = cell.GetArrayRange();
            
            // Mostrar la información del rango de matriz
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // Imprimir los valores en el rango de matriz
            Console.WriteLine("\nValues in the array range:");
            for (int r = arrayRange.StartRow; r <= arrayRange.EndRow; r++)
            {
                for (int c = arrayRange.StartColumn; c <= arrayRange.EndColumn; c++)
                {
                    Console.Write(cells[r, c].Value + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


