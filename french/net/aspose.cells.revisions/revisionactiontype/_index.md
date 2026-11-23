---
title: "Enumération RevisionActionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Revisions.RevisionActionType enum. Représente le type d'action de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

Représente le type d'action de révision.

```csharp
public enum RevisionActionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Add | `0` | Ajouter une révision. |
| Delete | `1` | Supprimer la révision. |
| DeleteColumn | `2` | Révision de suppression de colonne. |
| DeleteRow | `3` | Révision de suppression de ligne. |
| InsertColumn | `4` | Révision d'insertion de colonne. |
| InsertRow | `5` | Révision d'insertion de ligne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Effectuer diverses opérations qui génèrent différents types de révisions
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // Vérifier si le classeur possède des révisions
            if (workbook.HasRevisions)
            {
                // Remarque : l'API originale ne fournit pas d'accès direct à la collection des révisions
                // Nous allons donc simplement démontrer l'énumération RevisionActionType comme demandé
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // Démontrer l'utilisation des valeurs de l'énumération RevisionActionType
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // Enregistrez le classeur
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


