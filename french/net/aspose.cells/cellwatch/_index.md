---
title: "Classe CellWatch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CellWatch. Représente l'élément Cell Watch dans la fenêtre de surveillance"
type: docs
url: /fr/net/aspose.cells/cellwatch/
---
## CellWatch class

Représente le Cell Watch Item dans la 'fenêtre de surveillance'.

```csharp
public class CellWatch
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CellWatch](cellwatch/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Obtient et définit le nom de la cellule. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Obtient et définit la colonne de la cellule. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Obtient et définit la ligne de la cellule. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            // Obtenez la première feuille de calcul.
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez l'élément Cell Watch dans la fenêtre de surveillance
            int watchIndex = sheet.CellWatches.Add("B2");

            // Récupérez l'objet CellWatch
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Définition des propriétés
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Enregistrez le classeur
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


