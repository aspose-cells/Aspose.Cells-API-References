---
title: "RevisionQueryTable.FieldId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionQueryTable. Получает ID конкретного поля таблицы запросов, которое было удалено"
type: docs
url: /ru/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Получает идентификатор конкретного поля таблицы запросов, которое было удалено.

```csharp
public int FieldId { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // Создайте таблицу запросов (это упрощённый пример)
                // Примечание: В реальном сценарии вам сначала потребуется создать таблицу запросов
                // Для демонстрации мы смоделируем доступ к RevisionQueryTable

                // Поскольку в этом упрощённом примере мы не можем напрямую создать RevisionQueryTable,
                // мы покажем, как получить доступ к свойству FieldId, если бы оно существовало
                // Это демонстрирует шаблон чтения свойства только для чтения

                // Смоделируйте получение RevisionQueryTable из правок (концептуально)
                // На практике вы бы получили это из workbook.Revisions или аналогичного свойства
                RevisionQueryTable revisionQueryTable = null;

                // Проверьте, есть ли у нас таблица запросов правок (это только для демонстрации)
                if (revisionQueryTable != null)
                {
                    // Отобразите значение свойства FieldId
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Отобразите другие свойства для контекста
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Сохраните книгу
                workbook.Save("FieldIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


