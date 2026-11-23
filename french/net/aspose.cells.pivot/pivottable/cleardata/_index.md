---
title: "PivotTable.ClearData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Effacer les données et le formatage de la vue PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/cleardata/
---
## PivotTable.ClearData method

Efface les données et le formatage de la vue PivotTable.

```csharp
public void ClearData()
```

### Remarques

Si cette méthode n'est pas appelée avant d'ajouter ou de supprimer un PivotField, il se peut que les données du tableau croisé dynamique ne soient pas correctes

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodClearDataDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(15);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table with data:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Effacer les données du tableau croisé dynamique
            pivotTable.ClearData();
            Console.WriteLine("\nAfter ClearData():");
            Console.WriteLine("Pivot table row count: " + (pivotTable.DataBodyRange.EndRow - pivotTable.DataBodyRange.StartRow + 1));

            // Reconstruire le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nRebuilt pivot table:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Enregistrer le classeur
            workbook.Save("PivotTableClearDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


