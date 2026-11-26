---
title: "Cells.ImportFormulaArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa una matriz de fórmulas en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/importformulaarray/
---
## Cells.ImportFormulaArray method

Importa una matriz de formula a una hoja de cálculo.

```csharp
public void ImportFormulaArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringArray | String[] | Matriz de fórmulas. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| isVertical | Booleano | Especifica si se importan los datos verticalmente u horizontalmente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Preparar la matriz de fórmulas y los parámetros
            string[] formulas = new string[] { "=A1+B1", "=C1*D1" };
            int firstRow = 0;
            int firstColumn = 0;
            bool isVertical = true;

            try
            {
                // Importar fórmulas verticalmente comenzando en la celda A1
                worksheet.Cells.ImportFormulaArray(formulas, firstRow, firstColumn, isVertical);
                
                // Establecer valores para referencias de fórmulas
                worksheet.Cells["A1"].PutValue(2);
                worksheet.Cells["B1"].PutValue(3);
                worksheet.Cells["C1"].PutValue(4);
                worksheet.Cells["D1"].PutValue(5);
                
                // Calcular fórmulas
                workbook.CalculateFormula();

                Console.WriteLine("Formulas imported successfully. Calculated results:");
                Console.WriteLine($"A2 value: {worksheet.Cells["A2"].Value}"); // Should be 5
                Console.WriteLine($"A3 value: {worksheet.Cells["A3"].Value}"); // Should be 20
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportFormulaArray method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


