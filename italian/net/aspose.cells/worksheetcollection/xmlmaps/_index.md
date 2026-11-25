---
title: "WorksheetCollection.XmlMaps"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Ottiene e imposta le mappe XML nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Ottiene e imposta le mappe XML nella cartella di lavoro.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una mappa XML di esempio
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // Aggiungi la mappa XML alla cartella di lavoro
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // Accedi alla mappa XML
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Esporta dati XML (dimostra l'uso della proprietà XmlMaps)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### Vedi anche

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


