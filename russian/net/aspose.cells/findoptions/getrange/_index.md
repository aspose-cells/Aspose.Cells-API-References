---
title: "FindOptions.GetRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FindOptions. Получает и задает искомый диапазон"
type: docs
url: /ru/net/aspose.cells/findoptions/getrange/
---
## FindOptions.GetRange method

Получает и задает диапазон поиска.

```csharp
public CellArea GetRange()
```

### Возвращаемое значение

Возвращает искомый диапазон.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsMethodGetRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue("Grape");
            worksheet.Cells["B3"].PutValue("Lemon");

            // Создайте экземпляр FindOptions
            FindOptions findOptions = new FindOptions();
            findOptions.LookInType = LookInType.Values;
            findOptions.LookAtType = LookAtType.Contains;

            // Установите диапазон поиска в A1:B3
            CellArea searchArea = new CellArea();
            searchArea.StartRow = 0;
            searchArea.StartColumn = 0;
            searchArea.EndRow = 2;
            searchArea.EndColumn = 1;
            findOptions.SetRange(searchArea);

            try
            {
                // Получите установленный диапазон
                CellArea resultRange = findOptions.GetRange();

                // Отобразите информацию о диапазоне
                Console.WriteLine($"Search range: StartRow={resultRange.StartRow}, StartColumn={resultRange.StartColumn}, " +
                    $"EndRow={resultRange.EndRow}, EndColumn={resultRange.EndColumn}");

                // Выполните операцию поиска, чтобы продемонстрировать использование диапазона
                Cell foundCell = worksheet.Cells.Find("an", null, findOptions);
                if (foundCell != null)
                {
                    Console.WriteLine($"Found value '{foundCell.StringValue}' at {foundCell.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("MethodGetRangeDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


