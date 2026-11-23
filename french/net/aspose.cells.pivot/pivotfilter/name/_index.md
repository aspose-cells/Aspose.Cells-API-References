---
title: "PivotFilter.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Obtient le nom du filtre pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/name/
---
## PivotFilter.Name property

Obtient le nom du filtre pivot.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplit la feuille de calcul avec des données d'exemple
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ajoutez et configurez un filtre pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Name = "ProductFilter"; // Demonstrating Name property usage
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Actualisez et calculez les données du pivot
            pivot.RefreshData();
            pivot.CalculateData();

            // Enregistrez le classeur
            book.Save("PivotFilterNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


