---
title: "ExternalLinkCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalLinkCollection. Возвращает элемент ExternalLink по указанному индексу"
type: docs
url: /ru/net/aspose.cells/externallinkcollection/item/
---
## ExternalLinkCollection indexer

Возвращает элемент [`ExternalLink`](../../externallink/) по указанному индексу.

```csharp
public ExternalLink this[int index] { get; }
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
    public class ExternalLinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу с примерными внешними ссылками
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте несколько внешних ссылок
            worksheet.Cells["A1"].Formula = "='C:\\Temp\\External1.xlsx'!A1";
            worksheet.Cells["A2"].Formula = "='C:\\Temp\\External2.xlsx'!B2";
            
            // Получить доступ к внешним ссылкам с помощью свойства Item
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                ExternalLink link = workbook.Worksheets.ExternalLinks[i];
                Console.WriteLine($"External Link {i + 1}:");
                Console.WriteLine($"- DataSource: {link.DataSource}");
                Console.WriteLine($"- OriginalDataSource: {link.OriginalDataSource}");
            }
        }
    }
}
```

### См. также

* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


