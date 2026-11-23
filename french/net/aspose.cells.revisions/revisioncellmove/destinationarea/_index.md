---
title: "RevisionCellMove.DestinationArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellMove. Obtient la zone de destination"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellmove/destinationarea/
---
## RevisionCellMove.DestinationArea property

Obtient la zone de destination.

```csharp
public CellArea DestinationArea { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionCellMovePropertyDestinationAreaDemo
    {
        public static void Run()
        {
            // Créez un classeur pour disposer d'un environnement valide (facultatif pour la démo)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Demo";

            try
            {
                // Instanciez RevisionCellMove via la réflexion (constructeur sans paramètres)
                RevisionCellMove revMove = (RevisionCellMove)Activator.CreateInstance(typeof(RevisionCellMove));

                // Lisez et affichez la propriété DestinationArea (lecture seule)
                CellArea destination = revMove.DestinationArea;
                Console.WriteLine("DestinationArea: " + destination.ToString());

                // Contexte supplémentaire (facultatif)
                Console.WriteLine("SourceArea: " + revMove.SourceArea.ToString());
                Console.WriteLine("Revision Type: " + revMove.Type);

                // Enregistrez le classeur (facultatif)
                workbook.Save("RevisionCellMoveDestinationAreaDemo.xlsx");
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


