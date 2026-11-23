---
title: "PivotField.DragToData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique si le champ spécifié peut être glissé vers la région des valeurs. La valeur par défaut est true."
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/dragtodata/
---
## PivotField.DragToData property

Indique si le champ spécifié peut être glissé vers la région des valeurs. La valeur par défaut est true.

```csharp
[Obsolete("Use PivotField.AllowDraggingToData property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool DragToData { get; set; }
```

### Remarques

NOTE : Cette propriété est désormais obsolète. Veuillez plutôt utiliser la propriété PivotField.AllowDraggingToData. Cette méthode sera supprimée 12 mois après, à compter de juillet 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyDragToDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bikes";
            cells["A3"].Value = "Bikes";
            cells["A4"].Value = "Cars";
            cells["A5"].Value = "Cars";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 1500;
            cells["C4"].Value = 2000;
            cells["C5"].Value = 2500;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajoutez le champ de ligne et configurez DragToData
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];
            rowField.DragToData = true; // Allow dragging this field to data area
            
            // Ajouter un champ de colonne
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualiser le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotFieldDragToDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


