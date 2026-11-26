---
title: "Класс HighlightChangesOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.HighlightChangesOptions. Представляет параметры выделения ревизий или изменений в общих файлах Excel"
type: docs
url: /ru/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

Представляет параметры выделения ревизий или изменений в совместных файлах Excel.

```csharp
public class HighlightChangesOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Представляет параметры выделения ревизий или изменений в совместных файлах Excel. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // Создайте объект Workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Получить журналы ревизий
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Установить количество дней для сохранения истории
            revisionLogs.DaysPreservingHistory = 30;

            // Создать HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Выделить изменения
            revisionLogs.HighlightChanges(options);

            // Сохраните книгу с выделенными изменениями
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


