---
title: "Range.ClearHyperlinks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Удаляет только гиперссылки"
type: docs
url: /ru/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Только удаляет гиперссылки.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| clearFormat | Boolean | Указывает, следует ли очищать формат гиперссылок. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте диапазон и добавьте несколько гиперссылок для демонстрации
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Очистить гиперссылки с сохранением формата (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Снова добавить гиперссылки
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Очистить гиперссылки без сохранения формата (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Сохраните книгу
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


