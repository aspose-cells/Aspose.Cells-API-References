---
title: "ContentTypeProperty.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ContentTypeProperty. Возвращает или задает имя объекта"
type: docs
url: /ru/net/aspose.cells.properties/contenttypeproperty/name/
---
## ContentTypeProperty.Name property

Возвращает или задает имя объекта.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить свойство типа контента с именем "ss"
            workbook.ContentTypeProperties.Add("ss", "bb", "text");
            
            // Сохранить в формате XLS
            workbook.Save("example.xls");
            
            // Перезагрузить книгу и проверить свойство Name
            workbook = new Workbook("example.xls");
            Console.WriteLine("Name property in XLS: " + workbook.ContentTypeProperties[0].Name);
            
            // Сохранить в формате XLSX
            workbook.Save("example.xlsx");
            
            // Перезагрузить и снова проверить
            workbook = new Workbook("example.xlsx");
            Console.WriteLine("Name property in XLSX: " + workbook.ContentTypeProperties[0].Name);
        }
    }
}
```

### См. также

* class [ContentTypeProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


