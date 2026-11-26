---
title: "Класс RevisionDefinedName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionDefinedName. Представляет запись ревизии изменения определённого имени"
type: docs
url: /ru/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Представляет запись ревизии изменения определённого имени.

```csharp
public class RevisionDefinedName : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Получает формулу. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Получает старую формулу. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Получает текст определённого имени. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Представляет тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавить определённое имя в книгу
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Изменить определённое имя для создания ревизии
                definedName.RefersTo = "=Sheet1!$B$1";

                // Сохранить книгу для создания журналов ревизий
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Повторно открыть книгу для доступа к информации о ревизиях
                Workbook revisionWorkbook = new Workbook(filePath);

                // Итерировать журналы ревизий для поиска записей RevisionDefinedName
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // Отобразить свойства RevisionDefinedName
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


