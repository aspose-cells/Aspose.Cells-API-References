---
title: "PivotAreaFilter.Selected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotAreaFilter. Indique si ce champ a une sélection. Ne fonctionne que lorsque le tableau croisé dynamique est en vue Plan"
type: docs
url: /fr/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

Indique si ce champ a une sélection. Ne fonctionne que lorsque le tableau croisé dynamique est en vue Plan.

```csharp
public bool Selected { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtenir le filtre de zone de tableau croisé dynamique
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // Afficher la valeur Selected actuelle
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // Modifier la valeur Selected (n'affecte que la vue Plan)
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // Enregistrez le classeur
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


