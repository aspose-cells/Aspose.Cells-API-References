---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает язык документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

Получает или задает язык документа.

```csharp
public string Language { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Доступ к встроенной коллекции свойств документа
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Установите свойство language
            builtInProperties.Language = "en-US";

            // Установите другие базовые свойства для демонстрации
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // Сохраните книгу
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


