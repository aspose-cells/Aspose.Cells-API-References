---
title: "RevisionCustomView.ActionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionCustomView. Возвращает тип действия"
type: docs
url: /ru/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

Получает тип действия.

```csharp
public RevisionActionType ActionType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyActionTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Загрузите существующий workbook, который может содержать ревизии пользовательского вида
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Итерируйте все журналы ревизий в workbook
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Проверьте каждую ревизию в журнале
                    foreach (Revision revision in log.Revisions)
                    {
                        // Проверьте, является ли это ревизией пользовательского вида
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Отобразите значение свойства ActionType
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // Продемонстрируйте, как использовать свойство ActionType
                            switch (customViewRevision.ActionType)
                            {
                                case RevisionActionType.Add:
                                    Console.WriteLine("This revision represents adding a custom view");
                                    break;
                                case RevisionActionType.Delete:
                                    Console.WriteLine("This revision represents deleting a custom view");
                                    break;
                                default:
                                    Console.WriteLine("This revision represents another type of action");
                                    break;
                            }

                            // Отобразите дополнительные свойства для контекста
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");
                        }
                    }
                }
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


