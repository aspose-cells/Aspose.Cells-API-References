---
title: "WorksheetCollection.CustomDocumentProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Elektronik tabloyun tüm özel belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/customdocumentproperties/
---
## WorksheetCollection.CustomDocumentProperties property

Elektronik tabloyun tüm özel belge özelliklerini temsil eden bir [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Özel belge özellikleri ekle
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("CreatedDate", DateTime.Now);
            workbook.Worksheets.CustomDocumentProperties.Add("Version", 1.2);
            
            // Özelliklere eriş ve göster
            Console.WriteLine("Author: " + workbook.Worksheets.CustomDocumentProperties["Author"]);
            Console.WriteLine("Created: " + workbook.Worksheets.CustomDocumentProperties["CreatedDate"]);
            Console.WriteLine("Version: " + workbook.Worksheets.CustomDocumentProperties["Version"]);
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


