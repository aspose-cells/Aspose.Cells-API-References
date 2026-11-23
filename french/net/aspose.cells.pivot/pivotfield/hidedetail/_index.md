---
title: "PivotField.HideDetail"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Définit si le détail de tous les PivotItems d’un champ de tableau croisé dynamique est masqué. C’est-à-dire réduire/étendre ce champ"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Définit si le détail de tous les PivotItems d’un champ de tableau croisé dynamique est masqué. C’est-à-dire réduire/étendre ce champ.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isHiddenDetail | Boolean | Indique si le détail du champ de tableau croisé dynamique doit être masqué. |

### Remarques

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser les méthodes PivotItemsCollection.HideAllDetails() et UnhideAllDetails(). Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Masquer les détails pour le premier champ de ligne
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


