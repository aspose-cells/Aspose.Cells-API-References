---
title: "Cells.GetColumnWidthInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el ancho de la columna especificada en vista normal en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

Obtiene el ancho de la columna especificada en vista normal, en unidades de pulgadas.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna |

### Valor de retorno

Ancho de la columna

Ancho de la columna en vista normal.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetColumnWidth(int ,bool , CellsUnitType ). Este método será eliminado 12 meses después, a partir de abril de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer el ancho de la columna en pulgadas para demostración
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // Llamar a GetColumnWidthInch con parámetro Int32
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // Mostrar resultado
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


