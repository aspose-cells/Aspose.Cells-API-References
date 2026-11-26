---
title: "UnionRange.Hyperlinks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство UnionRange. Возвращает все гиперссылки в диапазоне"
type: docs
url: /ru/net/aspose.cells/unionrange/hyperlinks/
---
## UnionRange.Hyperlinks property

Получает все гиперссылки в диапазоне.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько гиперссылок в ячейки
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
            worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");

            // Создайте диапазон
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });

            // Получите гиперссылки в диапазоне
            Hyperlink[] hyperlinks = unionRange.Hyperlinks;
            Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);

            // Отобразите информацию о каждой гиперссылке
            foreach (Hyperlink link in hyperlinks)
            {
                Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
            }

            // Сохраните книгу
            workbook.Save("HyperlinksDemo.xlsx");
        }
    }
}
```

### См. также

* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


