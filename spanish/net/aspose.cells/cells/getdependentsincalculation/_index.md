---
title: "Cells.GetDependentsInCalculation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene todas las celdas cuyo resultado calculado depende de una celda específica"
type: docs
url: /es/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Obtiene todas las celdas cuyo resultado calculado depende de la celda específica.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda específica |
| columna | Int32 | Índice de columna de la celda específica. |
| recursivo | Booleano | Devuelve los dependientes que no hacen referencia directamente a la celda específica, sino a otras hojas de esa celda. |

### Valor de retorno

Enumerador para enumerar todos los dependientes (objetos Cell)

### Observaciones

Para usar este método, asegúrese de que el libro de trabajo se haya configurado con el valor true para [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) y se haya calculado completamente con esta configuración. Si no hay ninguna referencia de fórmula a esta celda, se devolverá null. Para más detalles y un ejemplo, consulte [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/)

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo y calcule las fórmulas
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Configure las dependencias de fórmulas:
            // C1 = 10 (valor de origen)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // Calcule las fórmulas para establecer dependencias
            workbook.CalculateFormula();

            try
            {
                // Obtenga los dependientes de la celda C1 (fila 0, columna 2) con verificación recursiva
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


