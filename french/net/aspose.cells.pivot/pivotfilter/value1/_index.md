---
title: "PivotFilter.Value1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Obtient la chaîne value1 du filtre pivot d'étiquette"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/value1/
---
## PivotFilter.Value1 property

Obtient la chaîne value1 du filtre pivot d'étiquette.

```csharp
public string Value1 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValue1Demo
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
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ajoutez un filtre pivot et définissez Value1
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Value1 = "Apple"; // Filter for Apple products only

            // Actualiser et calculer les données
            pivot.RefreshData();
            pivot.CalculateData();

            // Enregistrez le classeur
            book.Save("PivotFilterValue1Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


