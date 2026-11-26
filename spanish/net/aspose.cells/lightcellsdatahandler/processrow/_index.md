---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataHandler. Inicia el procesamiento de una fila"
type: docs
url: /es/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Comienza a procesar una fila.

```csharp
public bool ProcessRow(Row row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Row | Objeto fila que se está procesando actualmente. |

### Valor de retorno

si las celdas de esta fila necesitan ser procesadas. false para ignorar todas las celdas en esta fila.

### Observaciones

Se llamará después de que se hayan leído las propiedades de la fila, como altura, estilo, ...etc. Sin embargo, las celdas de esta fila aún no se han leído.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar datos de ejemplo
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // Crear controlador personalizado
                var handler = new CustomRowHandler();

                // Procesar la primera fila
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // Demostrar el acceso a las propiedades de la fila
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // Modificar la altura de la fila si no es la fila de encabezado
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Ver también

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


