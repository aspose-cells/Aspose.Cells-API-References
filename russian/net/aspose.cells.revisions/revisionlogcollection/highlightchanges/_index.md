---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод RevisionLogCollection. Выделяет изменения совместной рабочей книги"
type: docs
url: /ru/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

Выделяет изменения совместно используемой книги.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | HighlightChangesOptions | Установите параметры фильтрации, какие изменения следует отслеживать. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые примерные данные и ревизии
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Подсветить изменения с параметрами
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


