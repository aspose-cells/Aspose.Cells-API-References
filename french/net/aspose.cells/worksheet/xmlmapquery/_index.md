---
title: "Worksheet.XmlMapQuery"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Interroger les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML"
type: docs
url: /fr/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Interroge les zones de cellules qui sont mappées/liées au chemin spécifique de la carte XML.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | chemin de l'élément xml |
| xmlMap | XmlMap | Spécifiez une carte xml si vous souhaitez interroger le chemin spécifique au sein d'une carte spécifique |

### Valeur de retour

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Worksheet.GetAreasOfXmlMapQuery(). Cette propriété sera supprimée 12 mois plus tard à partir d'août 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodXmlMapQueryWithStringXmlMapDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une carte XML d'exemple
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Importer du XML pour créer la carte
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // Obtenir la carte XML
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // Interroger la carte XML
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Afficher les résultats
            if (cellAreas.Count > 0)
            {
                CellArea area = (CellArea)cellAreas[0];
                Console.WriteLine($"Found data at row {area.StartRow}, column {area.StartColumn}");
                Console.WriteLine($"Cell value: {worksheet.Cells[area.StartRow, area.StartColumn].StringValue}");
            }
        }
    }
}
```

### Voir aussi

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


