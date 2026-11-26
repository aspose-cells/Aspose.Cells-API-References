---
title: "DocumentProperty.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "DocumentProperty property. Возвращает имя свойства"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/name/
---
## DocumentProperty.Name property

Возвращает имя свойства.

```csharp
public string Name { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к свойствам документа
            BuiltInDocumentPropertyCollection builtInProps = workbook.BuiltInDocumentProperties;
            CustomDocumentPropertyCollection customProps = workbook.CustomDocumentProperties;
            
            // Добавьте пользовательское свойство и продемонстрируйте использование Name
            DocumentProperty authorProperty = customProps.Add("Author", "John Doe");
            Console.WriteLine("Property Name: " + authorProperty.Name);
            Console.WriteLine("Property Value: " + authorProperty.Value);
            
            // Получить доступ к встроенному свойству по имени
            DocumentProperty titleProperty = builtInProps["Title"];
            titleProperty.Value = "Sample Document";
            Console.WriteLine("Title Property Name: " + titleProperty.Name);
            Console.WriteLine("Title Property Value: " + titleProperty.Value);
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


