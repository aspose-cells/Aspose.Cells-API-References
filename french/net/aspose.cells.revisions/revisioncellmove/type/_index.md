---
title: "RevisionCellMove.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellMove. Représente le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

Représente le type de révision.

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

    public class RevisionCellMovePropertyTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Créez une instance de RevisionCellMove en utilisant la réflexion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Afficher la valeur de la propriété Type (lecture seule)
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Afficher le contexte supplémentaire (facultatif)
                Console.WriteLine("Source Area: " + cellMoveRev.SourceArea);
                Console.WriteLine("Destination Area: " + cellMoveRev.DestinationArea);

                // Enregistrer le classeur (facultatif)
                workbook.Save("RevisionCellMoveTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


