---
title: "Workbook.ContentTypeProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает список объектов ContentTypeProperty в рабочей книге"
type: docs
url: /ru/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Возвращает список объектов [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) в рабочей книге.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyContentTypePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Добавить простое строковое свойство
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // Добавить свойство даты и времени с указанием типа
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Сохраните книгу
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


