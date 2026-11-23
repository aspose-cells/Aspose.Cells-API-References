---
title: "WorksheetCollection.XmlMaps"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Obtient et définit les cartes XML dans le classeur"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/xmlmaps/
---
## WorksheetCollection.XmlMaps property

Obtient et définit les cartes XML dans le classeur.

```csharp
public XmlMapCollection XmlMaps { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyXmlMapsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une carte XML d'exemple
            string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
                                <xs:element name='Root'>
                                    <xs:complexType>
                                        <xs:sequence>
                                            <xs:element name='Item' type='xs:string'/>
                                        </xs:sequence>
                                    </xs:complexType>
                                </xs:element>
                            </xs:schema>";
            
            // Ajouter une carte XML au classeur
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            
            // Accéder à la carte XML
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            
            // Exporter les données XML (démontre l'utilisation de la propriété XmlMaps)
            workbook.ExportXml(map.Name, "output.xml");
            
            Console.WriteLine("XML exported successfully using XmlMaps property.");
        }
    }
}
```

### Voir aussi

* class [XmlMapCollection](../../xmlmapcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


