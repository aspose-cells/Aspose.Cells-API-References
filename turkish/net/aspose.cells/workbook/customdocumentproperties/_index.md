---
title: "Workbook.CustomDocumentProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Elektronik tablonun tüm özel belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür"
type: docs
url: /tr/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

Elektronik tabloyun tüm özel belge özelliklerini temsil eden bir [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Özel belge özellikleri ekle
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // Özel özelliklere erişin ve görüntüleyin
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


