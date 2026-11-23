---
title: "Classe ExternalLinkCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalLinkCollection. Représente la collection de liens externes dans un classeur"
type: docs
url: /fr/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Représente la collection de liens externes dans un classeur.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Obtient le nombre d'éléments réellement contenus dans la collection. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Obtient l'élément [`ExternalLink`](../externallink/) à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Ajoute un lien externe. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Ajoutez un lien externe . |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Supprime tous les liens externes. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Supprime tous les liens externes. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Obtenez un énumérateur qui parcourt cette collection. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Supprime le lien externe spécifié du classeur. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Supprime le lien externe spécifié du classeur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // Ouvrir un fichier avec des liens externes
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // Obtenez la collection de liens externes
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Affichez le nombre de liens externes
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // Parcourez les liens externes et affichez leurs sources de données
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // Ajoutez un nouveau lien externe
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // Modifiez la source de données du premier lien externe
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // Enregistrez le classeur
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // Effacez tous les liens externes
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // Enregistrez le classeur après avoir supprimé les liens externes
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


