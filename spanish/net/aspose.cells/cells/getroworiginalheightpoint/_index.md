---
title: "Cells.GetRowOriginalHeightPoint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la altura original de las filas en unidades de punto si la fila está oculta"
type: docs
url: /es/net/aspose.cells/cells/getroworiginalheightpoint/
---
## Cells.GetRowOriginalHeightPoint method

Obtiene la altura original de la fila en unidades de punto si la fila está oculta

```csharp
[Obsolete("Use Cells.GetRowHeight(int,bool,CellsUnitType) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetRowOriginalHeightPoint(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Cells.GetRowHeight(int,bool,CellsUnitType). Este método será eliminado 12 meses después desde abril de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowOriginalHeightPointWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Almacenar altura original antes de la modificación
            double originalHeightBefore = cells.GetRowOriginalHeightPoint(0);
            
            // Modificar la altura de la fila
            cells.SetRowHeight(0, 25.5);

            try
            {
                // Obtener la altura original después de la modificación
                double originalHeight = cells.GetRowOriginalHeightPoint(0);
                double currentHeight = cells.GetRowHeight(0);

                Console.WriteLine($"Original row height: {originalHeight} points");
                Console.WriteLine($"Current row height: {currentHeight} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowOriginalHeightPoint: {ex.Message}");
            }

            workbook.Save("GetRowOriginalHeightPointDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


