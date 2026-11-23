---
title: "Classe ExternalLink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalLink. Représente un lien externe dans un classeur"
type: docs
url: /fr/net/aspose.cells/externallink/
---
## ExternalLink class

Représente un lien externe dans un classeur.

```csharp
public class ExternalLink
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Représente la source de données du lien externe. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Indique si ce lien externe est référencé par d’autres. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Indique si ce lien externe est visible dans MS Excel. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Représente la source de données stockée du lien externe. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Obtenez le type de chemin de ce lien externe |
| [Type](../../aspose.cells/externallink/type/) { get; } | Obtient le type du lien externe. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Ajoute un nom externe. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // Ouvrir un fichier avec des liens externes
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Obtenir le lien externe 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Affiche les propriétés du lien externe
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Modifier la source de données du lien externe
            externalLink.DataSource = "d:\\linktest.xls";

            // Ajoutez un nom externe au lien externe
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Enregistrez le classeur
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


