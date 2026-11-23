---
title: "XmlMap.RootElementName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlMap. Obtient le nom de l’élément racine"
type: docs
url: /fr/net/aspose.cells/xmlmap/rootelementname/
---
## XmlMap.RootElementName property

Obtient le nom de l'élément racine.

```csharp
public string RootElementName { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyRootElementNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Créer une carte XML
            string xml = "<root><item><Name>Item1</Name><Value>100</Value></item></root>";
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xml);
            
            // Obtenir et afficher le nom de l’élément racine
            string rootElementName = workbook.Worksheets.XmlMaps[mapIndex].RootElementName;
            Console.WriteLine("Root Element Name: " + rootElementName);
        }
    }
}
```

### Voir aussi

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


