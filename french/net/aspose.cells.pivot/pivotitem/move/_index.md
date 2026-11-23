---
title: "PivotItem.Move"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotItem. Déplace l'élément vers le haut ou vers le bas"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

Déplace l'élément vers le haut ou vers le bas

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| décalage | Int32 | Le nombre de déplacements vers le haut ou vers le bas. Déplacez l'élément vers le haut si cette valeur est inférieure à zéro ; déplacez l'élément vers le bas si cette valeur est supérieure à zéro. |
| isSameParent | Boolean | Spécifie si l'opération de déplacement se trouve dans le même nœud parent ou non |

### Remarques

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode PivotTable.MoveItem(PivotFieldType, string[],bool,int) ou la méthode PivotItem.Move(int). Cette méthode sera supprimée 12 mois plus tard à partir de novembre 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Créer des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Obtenez les éléments pivot et démontrez la méthode Move
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // Déplacer le premier élément à la position 1 (deuxième position) avec les éléments enfants
            items[0].Move(1, true);
            
            // Enregistrez le classeur
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

Déplace l'élément vers le haut ou le bas dans le champ pivot

```csharp
public void Move(int offset)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| décalage | Int32 | Le nombre de déplacements vers le haut ou vers le bas. Déplacez l'élément vers le haut si cette valeur est inférieure à zéro ; déplacez l'élément vers le bas si cette valeur est supérieure à zéro. |

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


