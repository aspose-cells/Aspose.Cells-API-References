---
title: "PivotField.DragToPage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique si le champ spécifié peut être glissé vers la région de page. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/dragtopage/
---
## PivotField.DragToPage property

Indique si le champ spécifié peut être glissé vers la région des pages. La valeur par défaut est true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToPage { get; set; }
```

### Remarques

NOTE: Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToPage. Cette méthode sera supprimée 12 mois plus tard à compter de juillet 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToPageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Cars";
            cells["A4"].Value = "Bikes";
            cells["A5"].Value = "Cars";
            
            cells["B1"].Value = "Region";
            cells["B2"].Value = "North";
            cells["B3"].Value = "South";
            cells["B4"].Value = "North";
            cells["B5"].Value = "South";
            
            cells["C1"].Value = "Sales";
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter des champs et configurer DragToPage
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Page, "Region");
            PivotField regionField = pivotTable.PageFields[fieldIndex];
            
            // Démontrer la propriété DragToPage
            regionField.DragToPage = false; // Disable dragging to page area
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualiser le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrer le classeur
            workbook.Save("PivotFieldDragToPageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


