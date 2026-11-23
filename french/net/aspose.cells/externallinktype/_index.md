---
title: "Énumération ExternalLinkType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ExternalLinkType enum. Représente le type de lien externe"
type: docs
url: /fr/net/aspose.cells/externallinktype/
---
## ExternalLinkType enumeration

Représente le type de lien externe.

```csharp
public enum ExternalLinkType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DDELink | `0` | Représente le lien DDE. |
| External | `1` | Représente un lien externe. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkTypeDemo
    {
        public static void ExternalLinkTypeExample()
        {
            // Ouvrir un fichier avec des liens externes
            Workbook workbook = new Workbook("ExternalLinkTypeExample_original.xlsx");

            // Obtenir le lien externe 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Afficher le type de lien externe
            Console.WriteLine("External Link Type: " + externalLink.Type);

            // Modifier la source de données du lien externe
            externalLink.DataSource = "d:\\link.xls";

            // Enregistrez le classeur
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }

    // Énumération représentant le type de lien externe
    public enum ExternalLinkType
    {
        DDELink = 0, // Represents the DDE link
        External = 1 // Represents external link
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


