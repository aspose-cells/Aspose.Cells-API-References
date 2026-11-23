---
title: "RevisionCellChange.IsOldFormatted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellChange. Indique si cette cellule est formatée à l'ancienne"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellchange/isoldformatted/
---
## RevisionCellChange.IsOldFormatted property

Indique si cette cellule est anciennement formatée.

```csharp
public bool IsOldFormatted { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsOldFormattedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la valeur et le style initiaux de la cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            cell.SetStyle(initialStyle);

            // Modifier la valeur et le style de la cellule pour créer une révision
            cell.PutValue("Updated Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Calibri";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            try
            {
                // Accédez aux journaux de révision
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Afficher la valeur de la propriété IsOldFormatted
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);

                            // Afficher un contexte supplémentaire sur la révision
                            if (cellChange.IsOldFormatted)
                            {
                                Console.WriteLine("The cell had formatting before this revision.");
                                Console.WriteLine("Old Font: " + cellChange.OldStyle.Font.Name);
                                Console.WriteLine("Old Font Size: " + cellChange.OldStyle.Font.Size);
                            }
                            else
                            {
                                Console.WriteLine("The cell did not have formatting before this revision.");
                            }
                        }
                    }
                }

                // Enregistrer le classeur avec les révisions
                workbook.Save("IsOldFormattedDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved as IsOldFormattedDemo.xlsx");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


