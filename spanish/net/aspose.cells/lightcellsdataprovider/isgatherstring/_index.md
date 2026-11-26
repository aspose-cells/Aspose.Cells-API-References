---
title: "LightCellsDataProvider.IsGatherString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataProvider. Verifica si el valor de cadena actual de la celda necesita recopilarse en un pool global"
type: docs
url: /es/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Comprueba si el valor de cadena actual de la celda necesita recopilarse en un pool global.

```csharp
public bool IsGatherString()
```

### Valor de retorno

true si el valor de cadena necesita recopilarse en un pool global para el archivo resultante.

### Observaciones

Recopilar valores de cadena solo será ventajoso cuando haya muchos valores de cadena duplicados en las celdas proporcionadas por esta implementación. En esta situación, recopilar cadenas ahorrará mucha memoria y generará un archivo resultante más pequeño. Si hay muchos valores de cadena en las celdas proporcionadas por LightCellsDataProvider pero pocos son iguales, recopilar cadenas consumirá más memoria y tiempo y no tendrá ventaja para el archivo resultante.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodIsGatherStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with IsGatherString implementation");
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
            private readonly object[,] data = new object[3, 2]
            {
                { "Product", "Price" },
                { "Laptop", 1200.50 },
                { "Phone", 899.99 }
            };

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 3 ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString()
            {
                // Recopilar solo cadenas para la fila de encabezado (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### Ver también

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


