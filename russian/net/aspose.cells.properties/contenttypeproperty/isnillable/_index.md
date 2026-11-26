---
title: "ContentTypeProperty.IsNillable"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ContentTypeProperty. Указывает, может ли значение быть пустым"
type: docs
url: /ru/net/aspose.cells.properties/contenttypeproperty/isnillable/
---
## ContentTypeProperty.IsNillable property

Указывает, может ли значение быть пустым.

```csharp
public bool IsNillable { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyIsNillableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Добавить свойство типа контента
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Получить доступ к свойству и установить IsNillable
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            property.IsNillable = true;
            
            // Проверить и вывести значение IsNillable
            Console.WriteLine($"Property 'Admin' IsNillable: {property.IsNillable}");
            
            workbook.Save("ContentTypePropertyIsNillableDemo.xlsx");
        }
    }
}
```

### См. также

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


