---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomDocumentPropertyCollection yöntemi. İçeriğe bağlanan yeni bir özel belge özelliği oluşturur"
type: docs
url: /tr/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

İçeriğe bağlanan yeni bir özel belge özelliği oluşturur.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin adı. |
| kaynak | String | Özelliğin kaynağı. Adlandırılmış aralığın adı olmalıdır. |

### Dönüş Değeri

Yeni oluşturulan özelliğin nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bağlanacak A1 hücresine bir değer ayarla
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Karşılaştırma için normal bir özellik ekle
            customProperties.Add("RegularProperty", "Static Value");
            
            // Bağlı bir özellik ekle
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // Bağlı değeri güncelle
            customProperties.UpdateLinkedRange();

            // Özellikleri göster
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


