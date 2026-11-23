---
title: "XmlSaveOptions.XmlMapName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlSaveOptions. Indique si la carte xml est exportée dans le fichier"
type: docs
url: /fr/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

Indique si la carte XML est exportée dans le fichier.

```csharp
public string XmlMapName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Créer une carte XML et l'ajouter au classeur
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // Créer XmlSaveOptions et définir XmlMapName
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // Enregistrer le classeur avec le mappage XML
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### Voir aussi

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


