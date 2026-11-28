---
title: "XmlMap sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.XmlMap sınıfı. Xml harita bilgilerini temsil eder"
type: docs
url: /tr/net/aspose.cells/xmlmap/
---
## XmlMap class

Xml harita bilgilerini temsil eder.

```csharp
public class XmlMap
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Bu haritanın bir [`XmlDataBinding`](../xmldatabinding/) alır. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Nesnenin adını döndürür veya ayarlar. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Kök öğe adını alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına örnek veri ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Örnek bir XML dizesinden bir XML haritası oluşturun
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Data'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' maxOccurs='unbounded'>
                                                <xs:complexType>
                                                    <xs:sequence>
                                                        <xs:element name='Name' type='xs:string'/>
                                                        <xs:element name='Value' type='xs:integer'/>
                                                    </xs:sequence>
                                                </xs:complexType>
                                            </xs:element>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // XML haritasını çalışma kitabına ekleyin
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Verileri haritayı kullanarak XML'e dışa aktarın
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


