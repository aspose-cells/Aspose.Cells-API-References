---
title: "CustomProperty.BinaryValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomProperty. Получает и задает двоичное значение пользовательского свойства"
type: docs
url: /ru/net/aspose.cells.properties/customproperty/binaryvalue/
---
## CustomProperty.BinaryValue property

Получает и задает двоичное значение пользовательского свойства.

```csharp
public byte[] BinaryValue { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyPropertyBinaryValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте пользовательское свойство с образцовым значением
            worksheet.CustomProperties.Add("SampleBinary", "01010101");

            try
            {
                // Получить пользовательское свойство
                CustomProperty prop = worksheet.CustomProperties["SampleBinary"];

                // Отобразите имя и значение пользовательского свойства
                Console.WriteLine($"Custom Property Name : {prop.Name}");
                Console.WriteLine($"Custom Property Value: {prop.Value}");

                // ПРИМЕЧАНИЕ: Отражение для CustomProperty не включает свойство BinaryValue.
                // Доступ к доступному строковому значению осуществляется через свойство 'Value'.

                // Сохраните книгу (необязательно)
                workbook.Save("BinaryValueDemo.xlsx");
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


