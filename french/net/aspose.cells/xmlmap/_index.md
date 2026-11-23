---
title: "Classe XmlMap"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.XmlMap. Représente les informations de la carte Xml"
type: docs
url: /fr/net/aspose.cells/xmlmap/
---
## XmlMap class

Représente les informations de la carte Xml.

```csharp
public class XmlMap
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DataBinding](../../aspose.cells/xmlmap/databinding/) { get; } | Obtient un [`XmlDataBinding`](../xmldatabinding/) de cette carte. |
| [Name](../../aspose.cells/xmlmap/name/) { get; set; } | Renvoie ou définit le nom de l'objet. |
| [RootElementName](../../aspose.cells/xmlmap/rootelementname/) { get; } | Obtient le nom de l'élément racine. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassXmlMapDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Créer une carte XML à partir d'une chaîne XML d'exemple
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
            
            // Ajouter la carte XML au classeur
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exporter les données en XML en utilisant la carte
            workbook.ExportXml(xmlMap.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMap.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


