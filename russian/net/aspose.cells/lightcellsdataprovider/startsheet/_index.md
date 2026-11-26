---
title: "LightCellsDataProvider.StartSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataProvider. Начинает сохранять рабочий лист"
type: docs
url: /ru/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Начинает сохранять лист.

```csharp
public bool StartSheet(int sheetIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | Индекс текущего листа, который будет сохранён. |

### Возвращаемое значение

true, если этот провайдер будет предоставлять данные для указанного листа; false, если указанный лист должен использовать свою обычную модель данных (Cells).

### Примечания

Он будет вызван в начале сохранения листа во время сохранения книги. Если провайдеру необходимо обратиться к

```csharp
sheetIndex
```

позже в методе startRow(Row) или startCell(Cell), то есть если процессу необходимо знать, какой лист обрабатывается, реализация должна сохранять

```csharp
sheetIndex
```

значение здесь.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartSheetWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                workbook.Worksheets.Clear(); // Start with clean worksheet
                
                // Создайте пользовательского поставщика данных и сохраните в режиме LightCells
                var saveOptions = new OoxmlSaveOptions
                {
                    LightCellsDataProvider = new CustomLightCellsDataProvider()
                };

                Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
                workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private bool sheetProcessed = false;

            // Вызывается при начале обработки листа
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // Обрабатывать только первый лист (индекс 0)
                if (sheetIndex == 0)
                {
                    sheetProcessed = true;
                    return true;
                }
                return false;
            }

            public int NextRow()
            {
                if (sheetProcessed)
                {
                    sheetProcessed = false;
                    return 0; // Process first row (index 0)
                }
                return -1; // Stop processing after first row
            }

            public void StartRow(Row row)
            {
                row.Height = 20;
            }

            public int NextCell()
            {
                return 0; // Process first cell (index 0)
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue("Data from LightCellsDataProvider");
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

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


