---
title: "LightCellsDataProvider.StartCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataProvider. Начинает сохранять данные одной ячейки"
type: docs
url: /ru/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

Начинает сохранять данные одной ячейки.

```csharp
public void StartCell(Cell cell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cell | Cell | Объект Cell для реализации заполнения данными. Его индекс столбца равен значению, возвращённому последним вызовом [`NextCell`](../nextcell/). Если ячейка была инициализирована во внутренней модели ячеек, будет использован существующий объект Cell. В противном случае будет использован временный объект Cell для заполнения данными. |

### Примеры

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
            
            // Создайте ячейку для использования в качестве параметра
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // Создайте пользовательского поставщика данных
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

### См. также

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


