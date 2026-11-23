---
title: "PivotField.IsAutoSort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique si les éléments de ce champ de tableau croisé dynamique sont triés automatiquement"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Indique si les éléments de ce champ de tableau croisé dynamique sont triés automatiquement.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoSort { get; set; }
```

### Remarques

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotField.SortSetting.SortType ou la méthode PivotField.SortBy() . Cette méthode sera supprimée 12 mois plus tard à compter de septembre 2026. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoSortDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Blueberry";
            cells["B5"].Value = 15;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Ajouter un champ de ligne et définir le tri automatique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsAutoSort = true;
            rowField.AutoSortField = 1; // Sort by Quantity (column B)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotFieldIsAutoSortDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


