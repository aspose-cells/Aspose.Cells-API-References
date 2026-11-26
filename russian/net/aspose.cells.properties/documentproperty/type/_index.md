---
title: "DocumentProperty.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DocumentProperty property. Получает тип данных свойства"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

Получает тип данных свойства.

```csharp
public PropertyType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к пользовательским свойствам документа (не встроенным)
            CustomDocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Добавьте пользовательские свойства с разными типами
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 5);
            properties.Add("IsApproved", true);
            
            // Продемонстрировать использование свойства Type
            Console.WriteLine("Document Properties and Their Types:");
            foreach (DocumentProperty prop in properties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}, Type: {prop.Type}");
            }
            
            // Получить доступ к конкретному свойству и проверить его тип
            DocumentProperty dateProp = properties["CreatedDate"];
            if (dateProp.Type == PropertyType.DateTime)
            {
                Console.WriteLine("\nCreatedDate is a DateTime property");
                Console.WriteLine($"Value as DateTime: {dateProp.ToDateTime()}");
            }
        }
    }
}
```

### См. также

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


