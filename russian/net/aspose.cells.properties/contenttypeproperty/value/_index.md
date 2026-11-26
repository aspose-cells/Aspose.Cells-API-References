---
title: "ContentTypeProperty.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ContentTypeProperty. Возвращает или задает значение свойства типа контента"
type: docs
url: /ru/net/aspose.cells.properties/contenttypeproperty/value/
---
## ContentTypeProperty.Value property

Возвращает или задает значение свойства типа содержимого.

```csharp
public string Value { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Добавить свойство типа контента
            workbook.ContentTypeProperties.Add("Admin", "InitialValue", "text");
            
            // Получить доступ и изменить значение свойства
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.Value = "Aspose"; // Demonstrating Value property usage
            
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


