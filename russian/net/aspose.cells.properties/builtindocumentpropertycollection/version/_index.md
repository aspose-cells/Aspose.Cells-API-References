---
title: "BuiltInDocumentPropertyCollection.Version"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Представляет номер версии приложения, создавшего документ"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/version/
---
## BuiltInDocumentPropertyCollection.Version property

Представляет номер версии приложения, создавшего документ.

```csharp
public string Version { get; set; }
```

### Примечания

Его формат "00.0000", например: 12.0000

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyVersionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить некоторые свойства документа
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Получить доступ и отобразить свойство Version
            string version = workbook.BuiltInDocumentProperties.Version;
            Console.WriteLine("Document Version: " + version);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


