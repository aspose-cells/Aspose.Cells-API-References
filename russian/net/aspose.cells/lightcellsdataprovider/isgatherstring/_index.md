---
title: "LightCellsDataProvider.IsGatherString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataProvider. Проверяет, нужно ли текущое строковое значение ячейки собрать в глобальный пул"
type: docs
url: /ru/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Проверяет, нужно ли текущое строковое значение ячейки собрать в глобальный пул.

```csharp
public bool IsGatherString()
```

### Возвращаемое значение

true, если строковое значение необходимо собрать в глобальный пул для результирующего файла.

### Примечания

Сбор строковых значений будет полезен только тогда, когда для ячеек, предоставляемых этой реализацией, имеется много дублирующихся строковых значений. В этой ситуации сбор строк сэкономит значительное количество памяти и создаст более маленький результирующий файл. Если для ячеек, предоставляемых LightCellsDataProvider, существует много строковых значений, но лишь немногие из них одинаковы, сбор строк потребует больше памяти и времени и не даст преимуществ для результирующего файла.

### Примеры

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
                // Собирать строки только для строки заголовка (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### См. также

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


