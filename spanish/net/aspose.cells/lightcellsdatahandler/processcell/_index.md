---
title: "LightCellsDataHandler.ProcessCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataHandler. Inicia el procesamiento de una celda"
type: docs
url: /es/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Comienza a procesar una celda.

```csharp
public bool ProcessCell(Cell cell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| celda | Celda | Objeto Cell que se está procesando actualmente |

### Valor de retorno

si esta celda necesita mantenerse en el modelo de celdas de la hoja actual. Normalmente debería ser false para que todas las celdas no se mantengan en memoria después de ser procesadas y así se ahorre memoria. Para algún propósito especial, como cuando el usuario necesita acceder a algunas celdas más tarde después de que todo el libro de trabajo haya sido procesado, el usuario puede hacer que este método devuelva true para mantener esas celdas especiales en el modelo Cells y acceder a ellas posteriormente mediante APIs como Cells[row, column]. Sin embargo, mantener los datos de celdas en el modelo Cells requerirá más memoria y si se mantienen todas las celdas, la lectura del archivo de plantilla en modo LightCells será igual que leerlo de forma normal.

### Observaciones

Se llamará después de que se haya leído los datos de una celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodProcessCellWithCellDemo
    {
        public static void Run()
        {
            try
            {
                // Crear archivo de datos temporal
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // Crear opciones de carga con un controlador de celdas ligeras personalizado
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Cargar libro de trabajo con controlador personalizado
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // Guardar resultados procesados
                workbook.Save("output.xlsx");
                Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
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
                return true; // Process all cells
            }

            public bool ProcessCell(Cell cell)
            {
                // Duplicar valores numéricos y marcar cadenas
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    cell.PutValue($"TEXT: {cell.StringValue}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


