---
title: "PivotField.HideItemDetail"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Définit si le PivotItem spécifique dans un champ de tableau croisé dynamique a les détails masqués"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Définit si le PivotItem spécifique dans un champ de tableau croisé dynamique a les détails masqués.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | l'index du pivotItem dans le pivotField. |
| isHiddenDetail | Boolean | si le PivotItem spécifique est masqué |

### Remarques

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems[int].IsDetailHidden. Cette méthode sera supprimée dans 12 mois, depuis août 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("SampleData.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter des champs aux zones
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Masquer le détail de l'élément à l'index 2 (East) avec isHidden=false
            pivotField.HideItemDetail(2, false);
            
            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


