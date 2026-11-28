---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomDocumentPropertyCollection yöntemi. Özel özelliklere bağlı tüm aralıkları günceller ve özel belge özelliğinin değerini kullanarak bağlı aralığın hücre değerini günceller."
type: docs
url: /tr/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Özel özelliklere bağlı tüm aralıkları günceller (özel belge özelliğinin değerini kullanarak bağlı aralığın hücre değerini günceller).

```csharp
public void UpdateLinkedRange()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bağlanacak A1 hücresine bir değer ayarla
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Bağlı bir özellik ekle
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Tüm bağlı özellikleri güncelle
            customProperties.UpdateLinkedRange();
            
            // Bağlı özelliğin değerini al ve göster
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Çalışma kitabını kaydedin
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


