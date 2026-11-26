---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор CustomFilterCollection. Создаёт новый экземпляр"
type: docs
url: /ru/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Создаёт новый экземпляр.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, установите FilterColumn.FilterType как FilterType.CustomFilters, затем получите FilterColumn.CustomFilters. Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Создайте новую CustomFilterCollection, используя конструктор
                CustomFilterCollection filters = new CustomFilterCollection();

                // Отобразите значение свойства And по умолчанию
                Console.WriteLine($"Default And property value: {filters.And}");

                // Конструктор создаёт пустую коллекцию
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Сохраните книгу
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


