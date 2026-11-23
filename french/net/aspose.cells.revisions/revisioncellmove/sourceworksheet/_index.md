---
title: "RevisionCellMove.SourceWorksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellMove. Obtient la feuille de calcul source"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellmove/sourceworksheet/
---
## RevisionCellMove.SourceWorksheet property

Obtient la feuille de calcul source.

```csharp
public Worksheet SourceWorksheet { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellMovePropertySourceWorksheetDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Créez une instance de RevisionCellMove en utilisant la réflexion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Affichez la valeur de la propriété SourceWorksheet (lecture seule)
                Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet);

                // Contexte supplémentaire (facultatif)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea);
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea);
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Enregistrer le classeur (facultatif)
                workbook.Save("SourceWorksheetDemo.xlsx");
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

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


