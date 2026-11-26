---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает информационное имя шаблона документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

Получает или задает информационное имя шаблона документа.

```csharp
public string Template { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установите свойство Template
            builtInProperties.Template = "Standard Template";

            // Установите другие базовые свойства для демонстрации
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // Сохраните книгу
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


