---
title: "UnionRange.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Возвращает или задаёт имя диапазона"
type: docs
url: /ru/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Получает или задает имя диапазона.

```csharp
public string Name { get; set; }
```

### Примечания

Именованные диапазоны поддерживаются. Например,

range.Name = "Sheet1!MyRange";

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // Создайте диапазоны и объедините их в объединённый диапазон
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Отобразите текущее значение свойства Name
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // Установите новое имя для объединённого диапазона
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // Продемонстрируйте, что имя можно изменить снова
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // Сохраните книгу
                workbook.Save("UnionRangeNameDemo.xlsx");
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

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


