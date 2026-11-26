---
title: "DocumentProperty.Source"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DocumentProperty property. Источник связанного контента"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

Связанный источник содержимого.

```csharp
public string Source { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к пользовательским свойствам документа
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // Добавьте свойства
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // Получите свойства и отобразите их источники
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // Сохраните книгу
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


