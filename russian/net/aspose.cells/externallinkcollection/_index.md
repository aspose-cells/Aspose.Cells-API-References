---
title: "Класс ExternalLinkCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ExternalLinkCollection. Представляет коллекцию внешних ссылок в книге"
type: docs
url: /ru/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Представляет коллекцию внешних ссылок в книге.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Получает количество элементов, фактически содержащихся в коллекции. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Получает элемент [`ExternalLink`](../externallink/) по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Добавляет внешнюю ссылку. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Добавить внешнюю ссылку . |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Удаляет все внешние ссылки. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Удаляет все внешние ссылки. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Получить перечислитель, который перебирает элементы этой коллекции. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Удаляет указанную внешнюю ссылку из книги. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Удаляет указанную внешнюю ссылку из книги. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // Открыть файл с внешними ссылками
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // Получить коллекцию внешних ссылок
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Отобразить количество внешних ссылок
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // Перебрать внешние ссылки и отобразить их источники данных
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // Добавить новую внешнюю ссылку
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // Изменить источник данных первой внешней ссылки
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // Сохраните книгу
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // Очистить все внешние ссылки
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // Сохранить книгу после очистки внешних ссылок
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


