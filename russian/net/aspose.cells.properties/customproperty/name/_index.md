---
title: "CustomProperty.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomProperty. Возвращает или задает имя объекта"
type: docs
url: /ru/net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Возвращает или задает имя объекта.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте пользовательское свойство с именем и значением
                worksheet.CustomProperties.Add("SampleName", "SampleValue");

                // Получить пользовательское свойство
                CustomProperty customProperty = worksheet.CustomProperties["SampleName"];

                // Отобразите текущее значение свойства Name (операция чтения)
                Console.WriteLine("Custom Property Name: " + customProperty.Name);

                // Установите новое значение для свойства Name
                customProperty.Name = "UpdatedName";
                Console.WriteLine("Updated Custom Property Name: " + customProperty.Name);

                // Сохраните книгу
                workbook.Save("NameDemo.xlsx");
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

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


