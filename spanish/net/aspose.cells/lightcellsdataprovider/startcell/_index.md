---
title: "LightCellsDataProvider.StartCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataProvider. Inicia el guardado de datos de una celda"
type: docs
url: /es/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

Comienza a guardar datos de una celda.

```csharp
public void StartCell(Cell cell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | Cell | Objeto Cell para que la implementación rellene datos. Su índice de columna es el valor devuelto de la última llamada a [`NextCell`](../nextcell/). Si la celda ha sido inicializada en el modelo interno de celdas, se utilizará el objeto Cell existente. De lo contrario, se usará un objeto Cell temporal para que la implementación rellene los datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartCellWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una celda para usar como parámetro
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // Crear proveedor de datos personalizado
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("StartCellWithCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with StartCell implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly int totalRows = 5;
            private readonly int totalCells = 3;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < totalRows ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < totalCells ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1}, Col {cell.Column + 1}");
            }

            public bool IsGatherString()
            {
                return false;
            }
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


