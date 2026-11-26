---
title: "RevisionQueryTable.CellArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionQueryTable. Получает расположение затронутой таблицы запросов"
type: docs
url: /ru/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Получает расположение затронутой таблицы запросов.

```csharp
public CellArea CellArea { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
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
                // В реальном сценарии вы бы получили правки из книги
                // Для демонстрации мы создадим концептуальный пример
                // Примечание: экземпляры RevisionQueryTable обычно получаются из ревизий книги
                RevisionQueryTable revisionQueryTable = null;

                // Проверьте, есть ли у нас таблица запросов правок
                if (revisionQueryTable != null)
                {
                    // Отобразите значение свойства CellArea (только для чтения)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Отобразите другие свойства для контекста
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Сохраните книгу
                workbook.Save("CellAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


