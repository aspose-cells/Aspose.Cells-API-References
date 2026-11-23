---
title: "RevisionCellMove.SourceArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellMove. Obtient la zone source"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Obtient la zone source.

```csharp
public CellArea SourceArea { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellMovePropertySourceAreaDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques cellules avec des données d'exemple
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // L'exemple original utilisait des fonctionnalités de suivi des révisions qui ne sont pas
                // faites partie de l'API reflétée (IsTrackChanges, MoveRows, Revisions).
                // Pour que le code soit prêt à la compilation, nous démontrons la SourceArea
                // propriété en créant une instance de RevisionCellMove via la réflexion.
                // -------------------------------------------------------------

                // Créez une instance de RevisionCellMove en utilisant la réflexion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Affichez la valeur de SourceArea (lecture seule)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Informations complémentaires liées (facultatif)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // SourceWorksheet peut être nul pour une instance nouvellement créée
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Enregistrer le classeur (facultatif)
                workbook.Save("RevisionCellMoveSourceAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


