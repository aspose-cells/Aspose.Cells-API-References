---
title: "Klass XmlMap"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.XmlMap-klass. Representerar Xml-kartinformation"
type: docs
url: /sv/net/aspose.cells/xmlmap/
---
## XmlMap class

Representerar information om Xml-karta.

```csharp
public class XmlMap
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Hämtar en [`XmlDataBinding`](../xmldatabinding/) för denna karta. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Returnerar eller anger namnet på objektet. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Hämtar rot-elementets namn. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata i det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Skapa en XML‑karta från en exempel‑XML‑sträng
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
            
            // Lägg till XML‑kartan i arbetsboken
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exportera data till XML med hjälp av kartan
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


