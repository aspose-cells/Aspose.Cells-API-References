---
title: "Classe RevisionCellChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Revisions.RevisionCellChange class. Représente la révision qui modifie les cellules"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

Représente la révision qui modifie les cellules.

```csharp
public class RevisionCellChange : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Obtient le nom de la cellule. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Obtient l'index de colonne de la cellule. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Indique si cette cellule est nouvellement formatée. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Indique si cette cellule est anciennement formatée. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Obtient l'ancienne formule. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Obtient le nouveau style de la cellule. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Obtient la nouvelle valeur de la cellule. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Obtient l'ancienne formule. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Obtient l'ancien style de la cellule. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Obtient l'ancienne valeur de la cellule. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Obtient l'index de ligne de la cellule. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Représente le type de révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionCellChangeDemo
    {
        public static void Run()
        {
            // Créer le répertoire de sortie s'il n'existe pas
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // Créer le classeur initial et activer le partage
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // Rouvrir le classeur pour effectuer des modifications suivies
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // Première révision : définir les valeurs initiales
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // Deuxième révision : modifier les valeurs
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // Charger le classeur pour accéder aux journaux de révisions
            Workbook workbook3 = new Workbook(filePath);
            
            // Traiter tous les journaux de révisions
            foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
            {
                foreach (Revision rev in log.Revisions)
                {
                    if (rev.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rev;
                        Console.WriteLine($"Revision Type: {rev.Type}");
                        Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
                        Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
                        Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
                        Console.WriteLine("------------------------------------");
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


