---
title: "PivotTable.SelectArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Sélectionnez une zone de la vue du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/selectarea/
---
## PivotTable.SelectArea method

Sélectionnez une zone de la vue du tableau croisé dynamique.

```csharp
public PivotAreaCollection SelectArea(CellArea ca)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | La zone de cellules. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodSelectAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calculer les données
            pivotTable.CalculateData();

            // Définissez la zone de cellules à sélectionner
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 5;
            area.EndColumn = 6;

            try
            {
                // Appelez la méthode SelectArea avec le paramètre CellArea
                PivotAreaCollection selectedAreas = pivotTable.SelectArea(area);
                
                Console.WriteLine("SelectArea method executed successfully. Selected areas count: " + selectedAreas.Count);
                
                // Enregistrer le classeur pour montrer l'effet
                workbook.Save("PivotTableSelectAreaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SelectArea method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotAreaCollection](../../pivotareacollection/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


