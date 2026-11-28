---
title: "DocumentProperty.IsLinkedToContent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentProperty özelliği. Bu özelliğin içeriğe bağlı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Bu özelliğin içeriğe bağlı olup olmadığını gösterir

```csharp
public bool IsLinkedToContent { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Hücrelere örnek veri ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // Bağlantılı özel belge özellikleri oluştur
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // IsLinkedToContent özelliğini al ve kontrol et
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // Hücre değerini güncelle ve bağlantılı özellikleri yenile
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Özelliğin güncellendiğini doğrulayın
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // Çalışma kitabını kaydedin
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


