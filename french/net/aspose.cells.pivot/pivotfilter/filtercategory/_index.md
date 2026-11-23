---
title: "PivotFilter.FilterCategory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Obtient la catégorie de ce filtre"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/filtercategory/
---
## PivotFilter.FilterCategory property

Obtient la catégorie de ce filtre.

```csharp
public FilterCategory FilterCategory { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyFilterCategoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créez des données d'exemple de tableau croisé dynamique
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                worksheet.Cells["B1"].Value = "Value";
                worksheet.Cells["B2"].Value = 100;
                worksheet.Cells["B3"].Value = 200;
                worksheet.Cells["B4"].Value = 300;

                // Créer un tableau croisé dynamique
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Ajoutez un champ de ligne en utilisant la méthode API appropriée
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                
                // Ajoutez un champ de données en utilisant la méthode API appropriée
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;
                dataField.DisplayName = "Total";

                // Ajoutez un filtre de légende au champ Catégorie
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Affichez la valeur de la propriété FilterCategory
                Console.WriteLine("FilterCategory value: " + pivotFilter.FilterCategory);

                workbook.Save("FilterCategoryDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [FilterCategory](../../../aspose.cells/filtercategory/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


