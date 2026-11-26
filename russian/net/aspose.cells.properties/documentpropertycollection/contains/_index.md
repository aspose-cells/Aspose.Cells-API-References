---
title: "DocumentPropertyCollection.Contains"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DocumentPropertyCollection. Возвращает true, если в коллекции существует свойство с указанным именем"
type: docs
url: /ru/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Возвращает true, если свойство с указанным именем существует в коллекции.

```csharp
public bool Contains(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства без учёта регистра. |

### Возвращаемое значение

true, если свойство существует в коллекции; иначе false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Проверьте, существует ли свойство \"RevisionNumber\" во встроенных свойствах документа
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // Добавьте пользовательское свойство и проверьте его наличие
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### См. также

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


