---
title: "XmlMapCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode XmlMapCollection. Ajoutez un XmlMap par l'url/chemin d'un fichier xml/xsd"
type: docs
url: /fr/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Ajoutez un [`XmlMap`](../../xmlmap/) à partir de l'url/chemin d'un fichier xml/xsd.

```csharp
public int Add(string url)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| url | String | url/chemin d'un fichier xml/xsd. |

### Valeur de retour

[`XmlMap`](../../xmlmap/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
            
            // Ajoutez des cartes XML en utilisant des schémas et des fichiers XML.
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


