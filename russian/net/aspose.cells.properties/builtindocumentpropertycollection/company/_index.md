---
title: "BuiltInDocumentPropertyCollection.Company"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Получает или задает свойство компании"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/company/
---
## BuiltInDocumentPropertyCollection.Company property

Получает или задает свойство компании.

```csharp
public string Company { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyCompanyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить встроенные свойства документа, включая Company
            workbook.BuiltInDocumentProperties.Title = "Annual Report";
            workbook.BuiltInDocumentProperties.Company = "Contoso Ltd";
            
            // Сохраните книгу
            workbook.Save("DocumentPropertiesDemo.xlsx");
            
            // Отобразить заданные свойства
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties.Title);
            Console.WriteLine("Company: " + workbook.BuiltInDocumentProperties.Company);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


