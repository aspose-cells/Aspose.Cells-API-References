---
title: "Класс RevisionRenameSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionRenameSheet. Представляет ревизию переименования листа"
type: docs
url: /ru/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Представляет ревизию переименования листа.

```csharp
public class RevisionRenameSheet : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Получает новое имя листа. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Получает старое имя листа. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Представляет тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Сохранить оригинальное имя и переименовать лист
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // Сохранить в поток памяти для создания ревизий
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Повторно открыть книгу, чтобы получить доступ к журналам ревизий
                workbook = new Workbook(ms);

                // Проверить журналы ревизий на наличие операции переименования
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Сохраните книгу
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


