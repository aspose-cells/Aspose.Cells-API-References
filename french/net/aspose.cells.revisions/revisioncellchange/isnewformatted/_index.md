---
title: "RevisionCellChange.IsNewFormatted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellChange. Indique si cette cellule est nouvellement formatée"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellchange/isnewformatted/
---
## RevisionCellChange.IsNewFormatted property

Indique si cette cellule est nouvellement formatée.

```csharp
public bool IsNewFormatted { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsNewFormattedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
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

            // Accédez aux journaux de révision
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Afficher les informations de révision
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Démontrer la propriété IsNewFormatted
                        Console.WriteLine("\nFormatting Information:");
                        Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);
                        Console.WriteLine("IsNewFormatted: " + cellChange.IsNewFormatted);

                        if (cellChange.IsNewFormatted)
                        {
                            Console.WriteLine("The cell has new formatting applied in this revision.");
                            Console.WriteLine("New Font: " + cellChange.NewStyle.Font.Name);
                            Console.WriteLine("New Font Size: " + cellChange.NewStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + cellChange.NewStyle.Font.IsBold);
                        }
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellChangePropertyIsNewFormattedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


