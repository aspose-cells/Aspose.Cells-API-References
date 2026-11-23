---
title: "PivotArea.GetCellAreas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotArea. Obtient les zones de cellules de cette zone pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotarea/getcellareas/
---
## PivotArea.GetCellAreas method

Obtient les zones de cellules de cette zone de tableau croisé dynamique.

```csharp
public CellArea[] GetCellAreas()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaMethodGetCellAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données de tableau croisé dynamique minimales
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";

            try
            {
                // Créer un tableau croisé dynamique avec une configuration de base
                int pivotIndex = worksheet.PivotTables.Add("A1:A3", "D1", "DemoPivotTable");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Initialiser la zone pivot avec l'instance du tableau croisé dynamique
                PivotArea pivotArea = new PivotArea(pivotTable);

                // Configurer les paramètres de la zone pivot
                pivotArea.RuleType = PivotAreaType.Normal;
                pivotArea.AxisType = PivotFieldType.Data;
                pivotArea.IsRowGrandIncluded = true;

                // Exécuter la méthode cible
                CellArea[] cellAreas = pivotArea.GetCellAreas();

                Console.WriteLine($"GetCellAreas returned {cellAreas.Length} cell area(s)");
                foreach (CellArea area in cellAreas)
                {
                    Console.WriteLine($"CellArea: Columns {area.StartColumn}-{area.EndColumn}, Rows {area.StartRow}-{area.EndRow}");
                }

                workbook.Save("GetCellAreasDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetCellAreas: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


