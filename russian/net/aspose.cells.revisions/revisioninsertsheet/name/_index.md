---
title: "RevisionInsertSheet.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionInsertSheet. Получает имя листа"
type: docs
url: /ru/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Получает имя листа.

```csharp
public string Name { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавьте новый лист, чтобы потенциально создать запись ревизии
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Смоделировать доступ к RevisionInsertSheet из правок
                // Примечание: В реальном сценарии это будет получено из workbook.Revisions
                // Для демонстрации создадим имитационный сценарий
                RevisionInsertSheet insertSheetRevision = null;

                // В реальном использовании вы бы получили это из коллекции правок
                // Например: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // Поскольку мы не можем создать RevisionInsertSheet напрямую, мы продемонстрируем
                // что вы бы сделали, если бы имели к нему доступ
                if (insertSheetRevision != null)
                {
                    // Отобразите значение свойства Name (только для чтения)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Продемонстрируйте использование свойства Name в условной проверке
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Сохраните книгу
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


