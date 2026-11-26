---
title: "LightCellsDataHandler.StartCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataHandler. Prepara el procesamiento de una celda"
type: docs
url: /es/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Prepara procesar una celda.

```csharp
public bool StartCell(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | índice de columna de la celda a procesar |

### Valor de retorno

si esta celda necesita ser procesada. false para ignorar la celda y comprobar la siguiente hasta alcanzar el final de los datos de celdas de la fila actual

### Observaciones

Se llamará al alcanzar una celda existente en la fila actual. La fila actual es la fila de la última llamada de [`ProcessRow`](../processrow/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodStartCellWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Crear un archivo de entrada temporal
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // Crear opciones de carga con un controlador de celdas ligeras personalizado
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Cargar libro de trabajo con controlador personalizado
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // Guardar el libro de trabajo procesado
                workbook.Save("output.xlsx");
                Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartCell method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartSheet(Worksheet sheet)
            {
                return true; // Process all sheets
            }

            public bool StartRow(int rowIndex)
            {
                return true; // Process all rows
            }

            public bool StartCell(int columnIndex)
            {
                // Procesar solo celdas en el índice de columna 1 (segunda columna)
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // Duplicar el valor de las celdas en la segunda columna
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true; // Continue processing
            }
        }
    }
}
```

### Ver también

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


