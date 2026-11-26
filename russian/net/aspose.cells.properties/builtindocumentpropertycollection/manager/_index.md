---
title: "BuiltInDocumentPropertyCollection.Manager"
second_title: "Справочник API Aspose.Cells для .NET"
description: "BuiltInDocumentPropertyCollection свойство. Получает или задает свойство менеджера"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/manager/
---
## BuiltInDocumentPropertyCollection.Manager property

Получает или задает свойство менеджера.

```csharp
public string Manager { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyManagerDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установите основные свойства документа, включая Manager
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Manager = "Jane Smith"; // Demonstrating Manager property usage
            builtInProperties.Company = "Aspose";

            // Сохраните книгу
            workbook.Save("DocumentPropertiesDemo.xlsx");

            Console.WriteLine("Workbook created with Manager property set to: " + builtInProperties.Manager);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


