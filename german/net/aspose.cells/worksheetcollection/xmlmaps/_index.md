---
title: "WorksheetCollection.XmlMaps"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Ruft die XML-Maps im Arbeitsbuch ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Ruft die XML‑Karten in der Arbeitsmappe ab und legt sie fest.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge eine Beispiel-XML-Map hinzu
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // Füge eine XML-Map zum Arbeitsbuch hinzu
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // Greife auf die XML-Map zu
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exportiere XML-Daten (demonstriert die Verwendung der XmlMaps-Eigenschaft)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### Siehe auch

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


