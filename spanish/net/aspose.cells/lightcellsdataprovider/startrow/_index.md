---
title: "LightCellsDataProvider.StartRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataProvider. Inicia el guardado de datos de una fila"
type: docs
url: /es/net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Comienza a guardar datos de una fila.

```csharp
public void StartRow(Row row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| row | Row | Objeto Row para que la implementación rellene datos. Su índice de fila es el valor devuelto de la última llamada a [`NextRow`](../nextrow/). Si la fila ha sido inicializada en el modelo interno de celdas, se utilizará el objeto Row existente. De lo contrario, se usará un objeto Row temporal para que la implementación rellene los datos. |

### Observaciones

Se llamará al comienzo de guardar una fila y los datos de sus celdas. Si la fila actual tiene algunas propiedades personalizadas como altura, estilo, ...etc., la implementación debe establecer esas propiedades en el objeto Row dado aquí.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartRowWithRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un proveedor de datos personalizado
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                // Procesar el libro de trabajo con nuestro proveedor de datos personalizado
                workbook.Save("StartRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook processed successfully with StartRow implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartRow method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int currentRow = -1;
            private readonly int totalRows = 5;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                currentRow++;
                return currentRow < totalRows ? currentRow : -1;
            }

            public void StartRow(Row row)
            {
                // Demostrar el método StartRow con el parámetro Row
                row.Height = 25;
                row.IsHidden = (currentRow % 2 == 0);
                Console.WriteLine($"Processing row {row.Index}, Height: {row.Height}, Hidden: {row.IsHidden}");
            }

            public int NextCell()
            {
                return 0; // Process only first cell in each row
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1} Data");
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

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


