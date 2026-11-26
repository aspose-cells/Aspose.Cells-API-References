---
title: "RevisionQueryTable.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство RevisionQueryTable. Представляет тип правки"
type: docs
url: /ru/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

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

    public class RevisionQueryTablePropertyTypeDemo
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

                // Создайте имитацию RevisionQueryTable (это концептуально — на практике вы бы получили её из правок)
                // Поскольку мы не можем напрямую создать экземпляр RevisionQueryTable, мы покажем шаблон
                RevisionQueryTable revisionQueryTable = null;

                // Проверьте, есть ли у нас таблица запросов правок
                if (revisionQueryTable != null)
                {
                    // Отобразите значение свойства Type (только для чтения)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Покажите значение перечисления как целое число для справки
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Отобразите другие свойства для контекста
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Сохраните книгу
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


