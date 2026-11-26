---
title: "ContentTypeProperty.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ContentTypeProperty. Получает и задает тип свойства"
type: docs
url: /ru/net/aspose.cells.properties/contenttypeproperty/type/
---
## ContentTypeProperty.Type property

Получает и задаёт тип свойства.

```csharp
public string Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Добавить свойства типа контента с разными типами
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            workbook.ContentTypeProperties.Add("Version", "1.0", "number");
            workbook.ContentTypeProperties.Add("Enabled", "true", "boolean");

            // Получить доступ и отобразить типы свойств
            foreach (ContentTypeProperty property in workbook.ContentTypeProperties)
            {
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}, Type: {property.Type}");
            }

            // Сохраните книгу
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


