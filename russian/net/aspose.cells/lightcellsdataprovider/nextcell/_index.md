---
title: "LightCellsDataProvider.NextCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataProvider. Получает следующую ячейку для сохранения"
type: docs
url: /ru/net/aspose.cells/lightcellsdataprovider/nextcell/
---
## LightCellsDataProvider.NextCell method

Получает следующую ячейку для сохранения.

```csharp
public int NextCell()
```

### Возвращаемое значение

индекс столбца следующей ячейки для сохранения. -1 означает, что достигнут конец данных текущей строки и дальнейшие ячейки текущей строки сохранять не нужно.

### Примечания

Он будет вызываться в начале сохранения одной ячейки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var provider = new DemoLightCellsDataProvider();
            XlsSaveOptions saveOptions = new XlsSaveOptions { LightCellsDataProvider = provider };

            try
            {
                workbook.Save("NextCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class DemoLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly object[,] data = new object[2, 2]
            {
                { "Column1", "Column2" },
                { 100, 200 }
            };

            public bool StartSheet(int sheetIndex) => sheetIndex == 0;

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 2 ? 1 : 0;
            }

            public void StartRow(Row row) { }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? 1 : 0;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString() => false;
        }
    }
}
```

### См. также

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


