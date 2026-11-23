---
title: "Cells.LinkToXmlMap"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Lien vers une carte XML"
type: docs
url: /fr/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Lien vers une carte XML.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mapName | String | nom de la carte XML |
| ligne | Int32 | ligne de la cellule de destination |
| column | Int32 | colonne de la cellule de destination |
| chemin | String | chemin de l'élément xml dans la carte xml |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Ajouter une carte XML d'exemple
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // Obtenir la première feuille de calcul
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Lier la cellule à la carte XML
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // Enregistrez le classeur
            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


