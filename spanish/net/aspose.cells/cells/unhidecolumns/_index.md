---
title: "Cells.UnhideColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Desoculta varias columnas"
type: docs
url: /es/net/aspose.cells/cells/unhidecolumns/
---
## Cells.UnhideColumns method

Muestra varias columnas.

```csharp
public void UnhideColumns(int column, int totalColumns, double width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |
| totalColumns | Int32 | Número de columna |
| ancho | Double | Ancho de columna. |

### Observaciones

Solo aplica el ancho de columna a las columnas ocultas.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUnhideColumnsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ocultar columnas 1-3 (basado en cero) inicialmente
            worksheet.Cells.HideColumns(1, 3);

            try
            {
                // Desocultar columnas comenzando en el índice 1 (segunda columna), con ancho de 3 columnas, establecer ancho a 15.5
                worksheet.Cells.UnhideColumns(1, 3, 15.5);

                // Verifique las columnas desocultadas comprobando su ancho
                Console.WriteLine($"Column 1 width after unhiding: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine("Columns 1-3 successfully unhidden with specified width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UnhideColumns: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("UnhideColumnsWithWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


