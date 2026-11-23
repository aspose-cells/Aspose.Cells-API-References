---
title: "PivotField.ItemCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient le nombre d'éléments de base dans ce champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/itemcount/
---
## PivotField.ItemCount property

Obtient le nombre d'éléments de base dans ce champ pivot.

```csharp
[Obsolete("Use PivotField.PivotItems.Count instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ItemCount { get; }
```

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.PivotItems.Count. Cette méthode sera supprimée 12 mois plus tard à compter d'août 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["A6"].PutValue("Fruit");
            worksheet.Cells["A7"].PutValue("Vegetable");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(120);
            worksheet.Cells["B6"].PutValue(180);
            worksheet.Cells["B7"].PutValue(90);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Obtenir le champ pivot et afficher son nombre d'éléments
            PivotField pivotField = pivotTable.RowFields[0];
            Console.WriteLine("Item count in pivot field: " + pivotField.ItemCount);
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldItemCountDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


