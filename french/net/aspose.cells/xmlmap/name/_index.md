---
title: "XmlMap.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlMap. Retourne ou définit le nom de l’objet"
type: docs
url: /fr/net/aspose.cells/xmlmap/name/
---
## XmlMap.Name property

Renvoie ou définit le nom de l'objet.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John Doe");
            
            // Ajouter une carte XML
            string xmlSchema = "<xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">" +
                "<xs:element name=\"Employee\">" +
                "<xs:complexType><xs:sequence>" +
                "<xs:element name=\"ID\" type=\"xs:int\"/>" +
                "<xs:element name=\"Name\" type=\"xs:string\"/>" +
                "</xs:sequence></xs:complexType></xs:element></xs:schema>";
                
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
            XmlMap map = workbook.Worksheets.XmlMaps[mapIndex];
            map.Name = "Employee";
            
            // Démontrer l’utilisation de la propriété Name
            Console.WriteLine("XML Map Name: " + map.Name);
            
            // Exporter vers XML en utilisant le nom de la carte
            string savePath = "output.xml";
            workbook.ExportXml(map.Name, savePath);
            
            Console.WriteLine("XML exported successfully to: " + savePath);
        }
    }
}
```

### Voir aussi

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


