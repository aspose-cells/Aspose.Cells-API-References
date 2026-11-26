---
title: "LightCellsDataProvider.NextRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LightCellsDataProvider. Obtiene la siguiente fila que se guardará"
type: docs
url: /es/net/aspose.cells/lightcellsdataprovider/nextrow/
---
## LightCellsDataProvider.NextRow method

Obtiene la siguiente fila a guardar.

```csharp
public int NextRow()
```

### Valor de retorno

el índice de la siguiente fila que se guardará. -1 indica que se ha alcanzado el final de los datos de la hoja actual y no hay más filas de la hoja actual que guardar.

### Observaciones

Se llamará al comienzo de guardar una fila y los datos de sus celdas (antes de [`StartRow`](../startrow/)).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            workbook.Worksheets.Add("Sheet1");

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            try
            {
                workbook.Save("LightCellsDataProviderMethodNextRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;
        private readonly int totalRows = 3;

        public bool StartSheet(int sheetIndex)
        {
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            currentCell = -1;
            return currentRow < totalRows ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            row.Height = 20;
        }

        public int NextCell()
        {
            currentCell++;
            return currentCell < 2 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Ver también

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


