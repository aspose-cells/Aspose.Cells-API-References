---
title: "PivotField.IsHiddenItemDetail"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Indique s'il faut masquer le détail du PivotItem spécifique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Indique s'il faut masquer le détail du PivotItem spécifique..

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItemDetail(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index du pivotItem dans le pivotField. |

### Valeur de retour

si le détail du PivotItem spécifique est masqué

### Remarques

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems[int].IsDetailHidden. Cette méthode sera supprimée dans 12 mois, depuis août 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtenir le champ pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Masquer le détail de l'élément pour l'index 1 (USA)
            pivotField.HideItemDetail(1, true);
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Vérifier si le détail de l'élément est masqué
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // Enregistrer le classeur
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


