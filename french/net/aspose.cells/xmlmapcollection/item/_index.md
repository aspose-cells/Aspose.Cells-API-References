---
title: "XmlMapCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlMapCollection. Obtient la carte xml selon l'index spécifié."
type: docs
url: /fr/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Obtient le xml map à l'index spécifié.

```csharp
public XmlMap this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

La carte xml

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accédez à XmlMapCollection depuis le classeur
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Ajoutez un nouveau XmlMap à la collection
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // Accédez au XmlMap en utilisant la propriété Item
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Affichez le nom du XmlMap
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // Enregistrez le classeur
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


