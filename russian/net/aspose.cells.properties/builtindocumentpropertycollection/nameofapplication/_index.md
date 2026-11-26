---
title: "BuiltInDocumentPropertyCollection.NameOfApplication"
second_title: "Справочник API Aspose.Cells для .NET"
description: "BuiltInDocumentPropertyCollection свойство. Получает или задает имя приложения"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/nameofapplication/
---
## BuiltInDocumentPropertyCollection.NameOfApplication property

Получает или задает имя приложения.

```csharp
public string NameOfApplication { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyNameOfApplicationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите свойство NameOfApplication
            workbook.BuiltInDocumentProperties.NameOfApplication = "Aspose.Cells Demo App";
            
            // Отобразите свойство NameOfApplication
            Console.WriteLine("Application Name: " + workbook.BuiltInDocumentProperties.NameOfApplication);
            
            // Сохраните книгу
            workbook.Save("output.ods");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


