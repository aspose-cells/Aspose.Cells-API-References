---
title: "CustomXmlPartCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomXmlPartCollection özelliği. Belirtilen indeksteki bir öğeyi alır"
type: docs
url: /tr/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

Belirtilen dizindeki bir öğeyi alır.

```csharp
public CustomXmlPart this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class CustomXmlPartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // CustomXmlPartCollection'a doğrudan Workbook'tan eriş
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Örnek XML verisi
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // Özel bir XML bölümü ekle
            int index = customXmlParts.Add(xmlBytes, null);
            
            // Öğeye Item özelliğini kullanarak erişin
            CustomXmlPart part = customXmlParts[index];
            
            // Özel XML bölümünün kimliğini göster
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // Bölümden XML verisini geri al
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


