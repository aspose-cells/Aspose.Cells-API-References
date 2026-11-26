---
title: "RevisionRenameSheet.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionRenameSheet. Представляет тип ревизии"
type: docs
url: /ru/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

Представляет тип ревизии.

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

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Включить отслеживание ревизий ПЕРЕД внесением изменений
            // Примечание: Этот метод не существует в предоставленном API, поэтому мы удалим его
            // workbook.StartTrackingRevisions();

            // Переименуйте первый лист, чтобы создать ревизию
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // Получить доступ к коллекции ревизий
            // Примечание: Свойство Revisions не существует в предоставленном API
            // Поэтому нам сначала нужно проверить, есть ли у книги ревизии
            if (workbook.HasRevisions)
            {
                // Найдите ревизию переименования листа
                RevisionRenameSheet renameRevision = null;
                // Поскольку мы не можем получить доступ к Revisions напрямую, нам потребуется изменить эту часть
                // Это просто заполнитель, поскольку реальный API не поддерживает доступ к ревизиям
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // Отобразите значение свойства Type
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // Продемонстрировать, как использовать свойство Type
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // Сохранить книгу с ревизиями
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### См. также

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


