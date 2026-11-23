---
title: "Cells.UnMerge"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Annule la fusion d'une plage spécifiée de cellules fusionnées"
type: docs
url: /fr/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Démarque une plage spécifiée de cellules fusionnées.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage (index zéro) |
| firstColumn | Int32 | Première colonne de cette plage (index zéro) |
| totalRows | Int32 | Nombre de lignes (indexé à 1) |
| totalColumns | Int32 | Nombre de colonnes (indexé à 1) |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fusionnez d'abord les cellules
            cells.Merge(0, 0, 2, 2);
            
            // Annulez la fusion des cellules précédemment fusionnées
            cells.UnMerge(0, 0, 2, 2);
            
            // Enregistrez le classeur
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


