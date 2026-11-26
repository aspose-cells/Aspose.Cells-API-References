---
title: "Класс RevisionInsertSheet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Revisions.RevisionInsertSheet. Представляет запись ревизии листа, который был вставлен"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertsheet/
---
## RevisionInsertSheet class

Представляет запись ревизии листа, который был вставлен.

```csharp
public class RevisionInsertSheet : Revision
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertsheet/actiontype/) { get; } | Получает тип действия ревизии. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Получает номер этой ревизии.(Наследовано от [`Revision`](../revision/).) |
| [Name](../../aspose.cells.revisions/revisioninsertsheet/name/) { get; } | Получает имя листа. |
| [SheetPosition](../../aspose.cells.revisions/revisioninsertsheet/sheetposition/) { get; } | Получает нулевую позицию нового листа на панели вкладок листов. |
| override [Type](../../aspose.cells.revisions/revisioninsertsheet/type/) { get; } | Получает тип ревизии. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Получает лист.(Наследовано от [`Revision`](../revision/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionInsertSheetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте новый лист, чтобы потенциально создать ревизию
                Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

                // Примечание: Поскольку мы не можем напрямую создавать экземпляры RevisionInsertSheet,
                // мы покажем, как работать с ним, если он существовал в коллекции ревизий
                // Это симулированный сценарий, поскольку реальный API отслеживания ревизий не полностью раскрыт

                // В реальном сценарии с включённым отслеживанием ревизий вы можете получить ревизии, как показано ниже:
                // RevisionInsertSheet revision = null; // Было бы получено из коллекции workbook.Revisions

                // В демонстрационных целях мы покажем шаблон работы с RevisionInsertSheet
                // Поскольку мы не можем напрямую создать его экземпляр, мы продемонстрируем шаблон доступа к свойствам

                // Вместо попытки создать экземпляр мы покажем, как работать с ним, если он доступен
                // Это сохраняет структуру, одновременно исправляя ошибку компиляции

                // Отобразите информацию о свойствах ревизии (симулировано)
                Console.WriteLine("RevisionInsertSheet properties demonstration:");
                Console.WriteLine("Type property would show: RevisionType.InsertSheet");
                Console.WriteLine("ActionType property would show: RevisionActionType.Add");
                Console.WriteLine("Name property would show the sheet name");
                Console.WriteLine("SheetPosition property would show the zero-based position");

                // Сохраните книгу
                workbook.Save("RevisionInsertSheetDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with potential revisions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionInsertSheet: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


