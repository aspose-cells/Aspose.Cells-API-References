---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFieldSortSetting. Indique si une opération de tri de données simple sera appliquée"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

Indique si une opération de tri de données simple sera appliquée.

```csharp
public bool IsSimpleSort { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
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
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtenir le champ pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // Obtenir le paramètre de tri (propriété en lecture seule)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Afficher la valeur actuelle de IsSimpleSort
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // Remarque : IsSimpleSort est en lecture seule, nous ne pouvons donc pas le définir directement
            // Pour démontrer le tri, nous créerons un nouveau tableau croisé dynamique avec un tri différent

            // Créer un autre tableau croisé dynamique avec un tri personnalisé
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Trier le champ du tableau croisé dynamique en utilisant la méthode disponible
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // Enregistrez le classeur
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


