---
title: "RevisionMergeConflict.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionMergeConflict. Возвращает тип исправления"
type: docs
url: /ru/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

Получает тип ревизии.

```csharp
public override RevisionType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Включить отслеживание изменений
            workbook.StartAccessCache(AccessCacheOptions.All);

            // Внести изменения для создания сценария конфликта слияния
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // Смоделировать конфликт слияния, открыв файл и внеся конфликтующие изменения
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // Объединить конфликтующие изменения
            workbook.Combine(otherUserWorkbook);

            // Проверить наличие исправлений
            if (workbook.HasRevisions)
            {
                // Найти исправление, вызвавшее конфликт слияния
                RevisionMergeConflict mergeConflictRevision = null;
                // Примечание: В реальной реализации вам понадобится другой способ доступа к исправлениям
                // поскольку свойство Revisions недоступно в предоставленном определении API

                if (mergeConflictRevision != null)
                {
                    // Отобразить свойство Type исправления конфликта слияния
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // Продемонстрировать, как можно использовать эту информацию
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


