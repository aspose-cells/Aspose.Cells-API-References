---
title: "WorksheetCollection.GetNamedRanges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Получает все предопределённые именованные диапазоны в таблице"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Получает все предопределённые именованные диапазоны в электронной таблице.

```csharp
public Range[] GetNamedRanges()
```

### Возвращаемое значение

Массив объектов Range. Если ссылка определённого имени внешняя или содержит несколько диапазонов, объект Range для этого имени не будет возвращён.

Возвращает null, если именованный диапазон не существует.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте несколько именованных диапазонов для демонстрации
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Вызовите метод GetNamedRanges, чтобы получить все именованные диапазоны
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Отобразите информацию об именованных диапазонах
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Сохраните книгу
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


