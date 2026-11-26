---
title: "LightCellsDataProvider.StartRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataProvider. Начинает сохранять данные одной строки"
type: docs
url: /ru/net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Начинает сохранять данные одной строки.

```csharp
public void StartRow(Row row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| row | Row | Объект Row для реализации заполнения данными. Его индекс строки равен значению, возвращённому последним вызовом [`NextRow`](../nextrow/). Если строка была инициализирована во внутренней модели ячеек, будет использован существующий объект Row. В противном случае будет использован временный объект Row для заполнения данными. |

### Примечания

Он будет вызываться в начале сохранения строки и данных её ячеек. Если у текущей строки есть пользовательские свойства, такие как высота, стиль, ... и т.д., реализация должна установить эти свойства в переданный объект Row здесь.

### Примеры

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
            
            // Создать пользовательского поставщика данных
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                // Обработать книгу с нашим пользовательским поставщиком данных
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
                // Продемонстрировать метод StartRow с параметром Row
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

### См. также

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


