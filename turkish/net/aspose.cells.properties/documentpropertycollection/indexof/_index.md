---
title: "DocumentPropertyCollection.IndexOf"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocumentPropertyCollection yöntemi. Bir özelliğin adına göre indeksini alır"
type: docs
url: /tr/net/aspose.cells.properties/documentpropertycollection/indexof/
---
## DocumentPropertyCollection.IndexOf method

Bir özelliğin adını kullanarak indeksini alır.

```csharp
public int IndexOf(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Özelliğin büyük/küçük harfe duyarsız adı. |

### Dönüş Değeri

Sıfır tabanlı indeks. Bulunamazsa negatif değer.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyCollectionMethodIndexOfWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yerleşik belge özellikleri koleksiyonunu al
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;

            // Yerleşik özellikler için yalnızca mevcut özelliklerin değerlerini ayarlayabiliriz
            // Özel özellikler eklemek için CustomDocumentPropertyCollection kullanmamız gerekir
            // Burada sadece gösterim amacıyla bazı mevcut yerleşik özellikleri ayarlayacağız
            properties["Title"].Value = "Value1";
            properties["Subject"].Value = "Value2";
            properties["Author"].Value = "Value3";

            try
            {
                // IndexOf yöntemini string parametresiyle çağır
                int index = properties.IndexOf("Subject");
                
                // Sonucu göster
                Console.WriteLine($"Index of 'Subject': {index}");
                
                // Bulunan indeksteki özelliği göster
                if (index >= 0)
                {
                    DocumentProperty property = properties[index];
                    Console.WriteLine($"Property at index {index}: {property.Name} = {property.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("DocumentPropertyIndexOfDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


