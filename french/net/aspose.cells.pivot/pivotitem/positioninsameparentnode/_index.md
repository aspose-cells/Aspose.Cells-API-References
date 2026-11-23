---
title: "PivotItem.PositionInSameParentNode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotItem. Spécifie l'index de position dans les PivotItems sous le même nœud parent"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/positioninsameparentnode/
---
## PivotItem.PositionInSameParentNode property

Spécifie l'index de position dans les PivotItems sous le même nœud parent.

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int PositionInSameParentNode { get; set; }
```

### Remarques

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode PivotTable.MoveItem(PivotFieldType, string[],bool,int). Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionInSameParentNodeDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Ajouter une nouvelle feuille de calcul pour le tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Configurer le tableau croisé dynamique
            PivotField vendorField = pivotTable.RowFields["Vendor"];
            vendorField.SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Actualiser et calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Démontrer la propriété PositionInSameParentNode
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Définir les positions au sein du même nœud parent
            items["4H12"].PositionInSameParentNode = 1;
            items["DIF400"].PositionInSameParentNode = 2;
            
            // Recalculer après avoir modifié les positions
            pivotTable.CalculateData();
            
            // Définir les positions pour un autre groupe
            items["CA32"].PositionInSameParentNode = 1;
            items["AAA3"].PositionInSameParentNode = 2;

            // Enregistrez le classeur
            workbook.Save("PivotTableWithPositionInSameParentNode.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


