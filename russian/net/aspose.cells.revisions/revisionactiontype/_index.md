---
title: "Перечисление RevisionActionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Revisions.RevisionActionType перечисление. Представляет тип действия ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

Представляет тип действия ревизии.

```csharp
public enum RevisionActionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Add | `0` | Добавить ревизию. |
| Delete | `1` | Удалить ревизию. |
| DeleteColumn | `2` | Ревизия удаления столбца. |
| DeleteRow | `3` | Ревизия удаления строки. |
| InsertColumn | `4` | Ревизия вставки столбца. |
| InsertRow | `5` | Ревизия вставки строки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Выполнить различные операции, генерирующие разные типы ревизий
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // Проверить, есть ли в книге ревизии
            if (workbook.HasRevisions)
            {
                // Примечание: оригинальный API не предоставляет прямой доступ к коллекции ревизий
                // Поэтому мы просто продемонстрируем перечисление RevisionActionType, как запрошено
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // Продемонстрировать использование значений перечисления RevisionActionType
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // Сохраните книгу
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


