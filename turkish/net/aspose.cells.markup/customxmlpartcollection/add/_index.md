---
title: "CustomXmlPartCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomXmlPartCollection yöntemi. Koleksiyona bir öğe ekler"
type: docs
url: /tr/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

Koleksiyona bir öğe ekler.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| veri | Byte[] | Bu Custom XML Data Storage Part'ın XML içeriği. |
| schemaData | Byte[] | Bu custom XML part ile ilişkili XML şemalarının kümesi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartCollectionMethodAddWithByteByteDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // CustomXmlPartCollection'ı doğrudan çalışma kitabından al
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // XML verisini ve şemayı bayt dizileri olarak hazırla
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // Add yöntemini bayt dizisi parametreleriyle çağır
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // Etkiyi göstermek için çalışma kitabını kaydedin
                workbook.Save("CustomXmlPartAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding custom XML part: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


