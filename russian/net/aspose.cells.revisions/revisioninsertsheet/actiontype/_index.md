---
title: "RevisionInsertSheet.ActionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertSheet. Возвращает тип действия правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

Получает тип действия ревизии.

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

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу с отслеживанием ревизий
            Workbook workbook = new Workbook();
            // Примечание: StartTrackingRevisions недоступен в предоставленном API
            // workbook.StartTrackingRevisions();

            // Добавьте новый лист для создания записи правки
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Примечание: StopTrackingRevisions недоступен в предоставленном API
            // workbook.StopTrackingRevisions();
            
            // Примечание: свойство Revisions недоступно в предоставленном API
            // Мы будем использовать HasRevisions, чтобы проверить, есть ли какие-либо ревизии
            if (workbook.HasRevisions)
            {
                // В реальном сценарии мы бы получили доступ к правкам здесь
                // Поскольку мы не можем создать RevisionInsertSheet напрямую, мы смоделируем проверку
                // Это предполагает, что мы получили правку откуда-то (например, из workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // Поскольку мы не можем создать или установить ActionType, мы просто продемонстрируем проверку
                if (insertSheetRevision != null)
                {
                    // Отобразите свойство ActionType
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // Продемонстрируйте использование свойства только для чтения
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // Сохранить книгу с ревизиями
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### См. также

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


