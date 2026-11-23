---
title: "Enum PivotTableSelectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Pivot.PivotTableSelectionType. Spécifie ce qui peut être sélectionné dans un tableau croisé dynamique lors d'une sélection structurée. Ces constantes peuvent être combinées pour sélectionner plusieurs types."
type: docs
url: /fr/net/aspose.cells.pivot/pivottableselectiontype/
---
## PivotTableSelectionType enumeration

Spécifie ce qui peut être sélectionné dans un tableau croisé dynamique lors d'une sélection structurée. Ces constantes peuvent être combinées pour sélectionner plusieurs types.

```csharp
public enum PivotTableSelectionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DataAndLabel | `0` | Données et libellés |
| DataOnly | `2` | Sélectionne uniquement les données |
| LabelOnly | `1` | Sélectionne uniquement les libellés |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableSelectionTypeDemo
    {
        public static void PivotTableSelectionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données au tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajoutez des champs au PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créer une PivotArea et définir ses propriétés
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Sélectionner la zone avec un type de sélection spécifique
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Enregistrez le classeur
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


