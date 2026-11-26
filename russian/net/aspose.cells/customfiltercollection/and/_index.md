---
title: "CustomFilterCollection.And"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomFilterCollection. Указывает, имеют ли два критерия отношение И"
type: docs
url: /ru/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

Указывает, имеют ли два критерия отношение "and".

```csharp
public bool And { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
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
                // Создайте новую CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Отобразите значение свойства And по умолчанию
                Console.WriteLine($"Default And property value: {filters.And}");

                // Установите свойство And в true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // Установите свойство And в false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Сохраните книгу
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


