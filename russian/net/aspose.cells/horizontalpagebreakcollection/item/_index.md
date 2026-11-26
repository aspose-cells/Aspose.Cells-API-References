---
title: "HorizontalPageBreakCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HorizontalPageBreakCollection. Получает элемент HorizontalPageBreak по указанному индексу"
type: docs
url: /ru/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Получает элемент [`HorizontalPageBreak`](../../horizontalpagebreak/) по указанному индексу.

```csharp
public HorizontalPageBreak this[int index] { get; }
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
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте горизонтальные разрывы страниц
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Получить разрывы страниц, используя свойство Item
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Изменять ячейки, которые влияют на разрывы страниц
            worksheet.Cells.DeleteRows(0, 2);
            
            // Проверьте, что разрыв страницы был скорректирован
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### См. также

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Получает элемент [`HorizontalPageBreak`](../../horizontalpagebreak/) с указанным именем ячейки.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
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
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте пару горизонтальных разрывов страниц, используя разные перегрузки
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- Доступ по целочисленному индексу (Item[int]) -----
                // Свойство Item является индексатором, поэтому мы используем синтаксис []
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- Доступ по строковому ключу (Item[string]) -----
                // Получите разрыв страницы, который был добавлен с именем ячейки "D5"
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // Сохраните книгу, чтобы проверить, что разрывы страниц сохранены
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


