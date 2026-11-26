---
title: "Класс CustomProperty"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Properties.CustomProperty class. Представляет пользовательское свойство, которое хранит пары имени и значения произвольных пользовательских данных для листа"
type: docs
url: /ru/net/aspose.cells.properties/customproperty/
---
## CustomProperty class

Представляет пользовательское свойство, которое хранит пары имя‑значение произвольных пользовательских данных для листа.

```csharp
public class CustomProperty
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BinaryValue](../../aspose.cells.properties/customproperty/binaryvalue/) { get; set; } | Получает и задает двоичное значение пользовательского свойства. |
| [Name](../../aspose.cells.properties/customproperty/name/) { get; set; } | Возвращает или задает имя объекта. |
| [StringValue](../../aspose.cells.properties/customproperty/stringvalue/) { get; set; } | (**Obsolete.**) Возвращает или задает значение пользовательского свойства. |
| [Value](../../aspose.cells.properties/customproperty/value/) { get; set; } | Возвращает или задает значение пользовательского свойства. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyDemo
    {
        public static void CustomPropertyExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Получить доступ к коллекции CustomProperties
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Добавить пользовательские свойства
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");
            customProperties.Add("LastModified", DateTime.Now.ToString());

            // Получить доступ и отобразить пользовательские свойства
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Сохраните книгу
            workbook.Save("CustomPropertyExample.xlsx");
            workbook.Save("CustomPropertyExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


