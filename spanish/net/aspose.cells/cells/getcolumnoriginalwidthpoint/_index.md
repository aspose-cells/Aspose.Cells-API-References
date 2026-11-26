---
title: "Cells.GetColumnOriginalWidthPoint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la altura original de la columna en unidades de punto si la columna está oculta"
type: docs
url: /es/net/aspose.cells/cells/getcolumnoriginalwidthpoint/
---
## Cells.GetColumnOriginalWidthPoint method

Obtiene la altura original de la columna en unidades de punto si la columna está oculta

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnOriginalWidthPoint(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | El índice de fila. |

### Valor de retorno

Ancho de la columna en vista normal.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetColumnWidth(int ,bool , CellsUnitType ). Este método será eliminado 12 meses después, a partir de abril de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnOriginalWidthPointWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Preparar el parámetro de índice de columna
            int columnIndex = 0;

            try
            {
                // Obtener el ancho original de la columna en puntos
                double originalWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width of column {columnIndex}: {originalWidth} points");

                // Modificar el ancho de la columna
                cells.SetColumnWidth(columnIndex, 15);
                Console.WriteLine("Set new column width to 15 points");

                // Obtener nuevamente el ancho original para demostrar que permanece sin cambios
                double unchangedWidth = cells.GetColumnOriginalWidthPoint(columnIndex);
                Console.WriteLine($"Original width remains: {unchangedWidth} points");

                // Obtener el ancho actual para mostrar la modificación
                double currentWidth = cells.GetColumnWidth(columnIndex);
                Console.WriteLine($"Current column width: {currentWidth} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnOriginalWidthPoint method: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("GetColumnOriginalWidthPointDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


