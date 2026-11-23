---
title: "PivotFilter.GetLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFilter. Obtient les libellés du filtre de légende"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/getlabels/
---
## PivotFilter.GetLabels method

Obtient les libellés du filtre de légende.

```csharp
public string[] GetLabels()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterMethodGetLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créez une structure de tableau croisé dynamique valide
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                
                // Créer un tableau croisé dynamique avec les paramètres corrects
                int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Créez un filtre pivot avec des paramètres valides
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Configurez les propriétés du filtre
                pivotFilter.Name = "SampleFilter";
                pivotFilter.EvaluationOrder = 1;

                // Exécutez la méthode GetLabels
                string[] labels = pivotFilter.GetLabels();

                Console.WriteLine($"Retrieved {labels?.Length ?? 0} labels:");
                if (labels != null)
                {
                    foreach (string label in labels)
                    {
                        Console.WriteLine($"- {label}");
                    }
                }

                workbook.Save("GetLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLabels: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


