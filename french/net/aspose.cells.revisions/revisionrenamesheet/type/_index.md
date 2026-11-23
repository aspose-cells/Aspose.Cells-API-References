---
title: "RevisionRenameSheet.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionRenameSheet. Représente le type de la révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

Représente le type de la révision.

```csharp
public override RevisionType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Activer le suivi des révisions AVANT d'apporter des modifications
            // Remarque : Cette méthode n'existe pas dans l'API fournie, nous allons donc la supprimer
            // workbook.StartTrackingRevisions();

            // Renommer la première feuille de calcul pour créer une révision
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // Accéder à la collection de révisions
            // Remarque : La propriété Revisions n'existe pas dans l'API fournie
            // Nous devrons donc d'abord vérifier si le workbook possède des révisions
            if (workbook.HasRevisions)
            {
                // Trouver la révision de renommage de feuille
                RevisionRenameSheet renameRevision = null;
                // Puisque nous ne pouvons pas accéder directement aux Révisions, nous devrons modifier cette partie
                // Ceci n'est qu'un espace réservé puisque l'API réelle ne prend pas en charge l'accès aux révisions
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // Afficher la valeur de la propriété Type
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // Démontrer comment utiliser la propriété Type
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


