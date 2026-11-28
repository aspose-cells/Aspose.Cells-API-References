---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomDocumentPropertyCollection yöntemi. İçeriğe bağlı tüm özel özelliklerin değerlerini günceller; bağlı aralığın hücre değerini kullanarak özel özelliğin değerini günceller."
type: docs
url: /tr/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

İçeriğe bağlı tüm özel özelliklerin değerlerini günceller (bağlı aralığın hücre değerini kullanarak özel özelliğin değerini günceller).

```csharp
public void UpdateLinkedPropertyValue()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Özel özelliklere bağlanacak hücrelere bazı veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Bağlı özel özellikler ekle
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Hücre değerlerini güncelle
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Bağlı özellik değerlerini güncelle
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Güncellenmiş özellik değerlerini göster
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


