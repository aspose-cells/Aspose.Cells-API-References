---
title: "WorksheetCollection.XmlMaps"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar och anger XML-kartor i arbetsboken"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Hämtar och anger XML-kartor i arbetsboken.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett exempel på XML-karta
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // Lägg till XML-karta i arbetsboken
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // Åtkomst till XML-kartan
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exportera XML-data (demonstrerar användning av XmlMaps-egenskapen)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### Se även

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


