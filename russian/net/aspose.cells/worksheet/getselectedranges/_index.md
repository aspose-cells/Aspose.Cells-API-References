---
title: "Worksheet.GetSelectedRanges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet method. Получает выбранные диапазоны ячеек в конструкторе таблицы"
type: docs
url: /ru/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Получает выбранные диапазоны ячеек в проектируемой таблице.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Возвращаемое значение

ArrayList, содержащий выбранные диапазоны.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Worksheet.GetSelectedAreas(). Это свойство будет удалено через 12 месяцев, начиная с марта 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Примечание: GetSelectedRanges помечен как устаревший в рефлексии
                // Это демонстрирует вызов метода, как запрошено
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Отобразить количество выбранных диапазонов
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Отобразить каждый выбранный диапазон
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Сохраните книгу
                workbook.Save("GetSelectedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


