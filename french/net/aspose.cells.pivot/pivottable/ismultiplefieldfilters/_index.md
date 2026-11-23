---
title: "PivotTable.IsMultipleFieldFilters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Spécifie une valeur booléenne qui indique si les champs d’un PivotTable peuvent avoir plusieurs filtres appliqués."
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/ismultiplefieldfilters/
---
## PivotTable.IsMultipleFieldFilters property

Spécifie une valeur booléenne qui indique si les champs d’un PivotTable peuvent avoir plusieurs filtres appliqués.

```csharp
[Obsolete("Use PivotTable.AllowMultipleFiltersPerField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsMultipleFieldFilters { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.AllowMultipleFiltersPerField. Cette méthode sera supprimée 12 mois plus tard, à compter de décembre 2024. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyIsMultipleFieldFiltersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("Fruit");
            worksheet.Cells["B3"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue("Fruit");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Afficher la valeur actuelle de IsMultipleFieldFilters
            Console.WriteLine("Current IsMultipleFieldFilters value: " + pivotTable.IsMultipleFieldFilters);

            // Définir IsMultipleFieldFilters sur true pour autoriser plusieurs filtres par champ
            pivotTable.IsMultipleFieldFilters = true;
            Console.WriteLine("IsMultipleFieldFilters set to: " + pivotTable.IsMultipleFieldFilters);

            // Actualisez et calculez le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTablePropertyIsMultipleFieldFiltersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


