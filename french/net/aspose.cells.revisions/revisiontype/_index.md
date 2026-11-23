---
title: "Énumération RevisionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "L'énumération Aspose.Cells.Revisions.RevisionType représente le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Représente le type de révision.

```csharp
public enum RevisionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| CustomView | `0` | Vue personnalisée. |
| DefinedName | `1` | Nom défini. |
| ChangeCells | `2` | Modification de cellules. |
| AutoFormat | `3` | Mise en forme automatique. |
| MergeConflict | `4` | Conflit de fusion. |
| Comment | `5` | Commentaire. |
| Format | `6` | Format. |
| InsertSheet | `7` | Insérer une feuille de calcul. |
| MoveCells | `8` | Déplacer des cellules. |
| Undo | `9` | Annuler. |
| QueryTable | `10` | Interroger le tableau. |
| InsertDelete | `11` | Insertion ou suppression. |
| RenameSheet | `12` | Renommer la feuille de calcul. |
| Unknown | `13` | Inconnu. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Démontrer l'utilisation de différentes valeurs d'énumération RevisionType
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Afficher les valeurs d'énumération et leurs valeurs entières sous-jacentes
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Démontrer la vérification des types de révision
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Enregistrez le classeur
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


