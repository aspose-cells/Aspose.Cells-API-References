---
title: "CustomProperty.StringValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomProperty. Возвращает или задает значение пользовательского свойства"
type: docs
url: /ru/net/aspose.cells.properties/customproperty/stringvalue/
---
## CustomProperty.StringValue property

Возвращает или задает значение пользовательского свойства.

```csharp
[Obsolete("Use CustomProperty.Value property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValue { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство CustomProperty.Value. Это свойство будет удалено через 12 месяцев, начиная с июня 2010 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyStringValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить пользовательское свойство со строковым значением
                worksheet.CustomProperties.Add("SampleProperty", "Test Value");

                // Получить пользовательское свойство
                CustomProperty customProperty = worksheet.CustomProperties["SampleProperty"];

                // Отобразить свойство StringValue (операция чтения)
                Console.WriteLine("StringValue: " + customProperty.StringValue);

                // Установить новое значение свойства StringValue
                customProperty.StringValue = "Updated Value";
                Console.WriteLine("Updated StringValue: " + customProperty.StringValue);

                // Сохраните книгу
                workbook.Save("StringValueDemo.xlsx");
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


