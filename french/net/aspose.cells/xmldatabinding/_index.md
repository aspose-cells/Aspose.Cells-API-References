---
title: "Classe XmlDataBinding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.XmlDataBinding. Représente les informations de liaison de données XML"
type: docs
url: /fr/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

Représente les informations de liaison de données Xml.

```csharp
public class XmlDataBinding
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Obtient l'URL source de cette liaison de données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un objet liste qui utilisera la liaison de données XML
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // Obtenir les informations de liaison de données XML (cela serait généralement défini lors de l'importation de données XML)
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // Afficher l'URL de la source de données XML (propriété en lecture seule)
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // Remarque : Dans un scénario réel, l'Url serait défini lors de l'importation des données XML
            // À des fins de démonstration, nous montrons comment accéder à la propriété

            // Enregistrez le classeur
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


