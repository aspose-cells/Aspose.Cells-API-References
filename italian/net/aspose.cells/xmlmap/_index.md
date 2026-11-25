---
title: "Classe XmlMap"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.XmlMap. Rappresenta le informazioni della mappa Xml"
type: docs
url: /it/net/aspose.cells/xmlmap/
---
## XmlMap class

Rappresenta le informazioni della mappa Xml.

```csharp
public class XmlMap
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Ottiene un [`XmlDataBinding`](../xmldatabinding/) di questa mappa. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Restituisce o imposta il nome dell'oggetto. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Ottiene il nome dell'elemento radice. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crea una mappa XML da una stringa XML di esempio
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
            
            // Aggiungi la mappa XML alla cartella di lavoro
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Esporta i dati in XML utilizzando la mappa
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


