---
title: "WorksheetCollection.XmlMaps"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Çalışma kitabındaki XML haritalarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Çalışma kitabındaki XML haritalarını alır ve ayarlar.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek bir XML haritası ekle
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // XML haritasını çalışma kitabına ekle
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // XML haritasına eriş
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // XML verilerini dışa aktar (XmlMaps özelliği kullanımını gösterir)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


