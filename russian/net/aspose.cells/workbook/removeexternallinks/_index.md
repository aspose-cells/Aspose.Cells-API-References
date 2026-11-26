---
title: "Workbook.RemoveExternalLinks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Удаляет все внешние ссылки в книге"
type: docs
url: /ru/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Удаляет все внешние ссылки в книге.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод ExternalLinkCollection.Clear(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2021 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Вызовите метод RemoveExternalLinks
                workbook.RemoveExternalLinks();

                // Отобразите результаты или эффекты вызова метода
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Сохраните книгу, если были внесены изменения
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


