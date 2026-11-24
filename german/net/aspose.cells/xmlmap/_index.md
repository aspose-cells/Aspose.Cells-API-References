---
title: "Klasse XmlMap"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.XmlMap Klasse. Stellt Informationen zur Xml-Karte dar"
type: docs
url: /de/net/aspose.cells/xmlmap/
---
## XmlMap class

Stellt Informationen zur XML‑Karte dar.

```csharp
public class XmlMap
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Ruft ein [`XmlDataBinding`](../xmldatabinding/) dieser Karte ab. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Gibt den Namen des Objekts zurück oder setzt ihn. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Ermittelt den Namen des Wurzelelements. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge Beispieldaten zum ersten Arbeitsblatt hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Erstelle eine XML-Map aus einer Beispiel-XML-Zeichenkette
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
            
            // Füge die XML-Map zur Arbeitsmappe hinzu
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exportiere Daten mithilfe der Map nach XML
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


