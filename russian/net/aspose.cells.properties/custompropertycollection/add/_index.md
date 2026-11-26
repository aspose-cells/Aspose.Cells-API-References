---
title: "CustomPropertyCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CustomPropertyCollection метод. Добавляет информацию о пользовательском свойстве"
type: docs
url: /ru/net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Добавляет информацию о пользовательском свойстве.

```csharp
public int Add(string name, string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя пользовательского свойства. |
| значение | String | Значение пользовательского свойства. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomPropertyCollection customProperties = worksheet.CustomProperties;
            
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            foreach (CustomProperty property in customProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            workbook.Save("CustomPropertiesExample.xlsx");
        }
    }
}
```

### См. также

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


