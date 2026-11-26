---
title: "BuiltInDocumentPropertyCollection.RevisionNumber"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает номер ревизии документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/revisionnumber/
---
## BuiltInDocumentPropertyCollection.RevisionNumber property

Получает или задает номер ревизии документа.

```csharp
public string RevisionNumber { get; set; }
```

### Примечания

Aspose.Cells не обновляет это свойство при изменении документа.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyRevisionNumberDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите свойство RevisionNumber
            workbook.BuiltInDocumentProperties.RevisionNumber = "1";
            
            // Отобразите RevisionNumber
            Console.WriteLine("Revision Number: " + workbook.BuiltInDocumentProperties.RevisionNumber);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


