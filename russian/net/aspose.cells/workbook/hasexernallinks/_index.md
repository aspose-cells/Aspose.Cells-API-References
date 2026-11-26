---
title: "Workbook.HasExernalLinks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Указывает, содержит ли эта рабочая книга внешние ссылки на другие источники данных"
type: docs
url: /ru/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Указывает, содержит ли эта рабочая книга внешние ссылки на другие источники данных.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Возвращаемое значение

Содержит ли эта рабочая книга внешние ссылки на другие источники данных.

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте ExternalLinkCollection.Count, чтобы проверить наличие внешних ссылок в этой рабочей книге. Этот метод будет удалён через 12 месяцев, начиная с декабря 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // Создать рабочую книгу с внешними ссылками
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // Добавить внешнюю ссылку
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // Проверить, содержит ли рабочая книга внешние ссылки
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


