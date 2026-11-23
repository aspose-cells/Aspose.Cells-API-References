---
title: "Workbook.RemoveExternalLinks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Supprime tous les liens externes du classeur"
type: docs
url: /fr/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Supprime tous les liens externes du classeur.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Remarques

NOTE: Ce membre est désormais obsolète. Veuillez plutôt utiliser la méthode ExternalLinkCollection.Clear(). Cette méthode sera supprimée 12 mois après décembre 2021. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour le contexte
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Appeler la méthode RemoveExternalLinks
                workbook.RemoveExternalLinks();

                // Afficher les résultats ou les effets de l'appel de la méthode
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Enregistrer le classeur si des modifications ont été apportées
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


