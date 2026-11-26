---
title: "VerticalPageBreakCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VerticalPageBreakCollection. Получает элемент VerticalPageBreak по указанному индексу"
type: docs
url: /ru/net/aspose.cells/verticalpagebreakcollection/item/
---
## VerticalPageBreakCollection indexer (1 of 2)

Получает элемент [`VerticalPageBreak`](../../verticalpagebreak/) по указанному индексу.

```csharp
public VerticalPageBreak this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить вертикальные разрывы страниц
            worksheet.VerticalPageBreaks.Add(5);
            worksheet.VerticalPageBreaks.Add(10);
            worksheet.VerticalPageBreaks.Add(15);

            // Получить доступ и отобразить разрывы страниц с помощью свойства Item
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < vpagebreaks.Count; i++)
            {
                Console.WriteLine($"Break {i + 1}: Column = {vpagebreaks[i].Column}");
            }

            // Удалите и добавьте заново, чтобы изменить разрыв страницы, так как Column доступен только для чтения
            int column = vpagebreaks[1].Column;
            vpagebreaks.RemoveAt(1);
            vpagebreaks.Add(12);
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine($"Break 2: Column = {vpagebreaks[1].Column}");
        }
    }
}
```

### См. также

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## VerticalPageBreakCollection indexer (2 of 2)

Получает элемент [`VerticalPageBreak`](../../verticalpagebreak/) с указанным именем ячейки.

```csharp
public VerticalPageBreak this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | Имя ячейки. |

### Возвращаемое значение

Элемент с указанным именем ячейки.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько вертикальных разрывов страниц
            worksheet.VerticalPageBreaks.Add(3);
            worksheet.VerticalPageBreaks.Add(7);

            try
            {
                // Получите доступ к VerticalPageBreakCollection
                VerticalPageBreakCollection pageBreaks = worksheet.VerticalPageBreaks;

                // Продемонстрировать доступ к элементам с использованием свойства Item (индексатор)
                Console.WriteLine("Vertical Page Breaks in the worksheet:");
                for (int i = 0; i < pageBreaks.Count; i++)
                {
                    VerticalPageBreak vpb = pageBreaks[i];
                    Console.WriteLine($"Break {i + 1}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
                }

                // Сохраните книгу
                workbook.Save("VerticalPageBreakItemDemo.xlsx");
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

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


