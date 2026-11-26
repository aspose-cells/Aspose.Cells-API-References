---
title: "BuiltInDocumentPropertyCollection.DocumentVersion"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Представляет версию файла"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/documentversion/
---
## BuiltInDocumentPropertyCollection.DocumentVersion property

Представляет версию файла.

```csharp
public string DocumentVersion { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyDocumentVersionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить свойство версии документа
            workbook.BuiltInDocumentProperties.DocumentVersion = "1.0";
            
            // Отобразить версию документа
            Console.WriteLine("Document Version: " + workbook.BuiltInDocumentProperties.DocumentVersion);
            
            // Сохраните книгу
            workbook.Save("DocumentVersionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


