---
title: "PivotField.GetFilters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotField method. Obtient tous les filtres pivot appliqués à ce champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/getfilters/
---
## PivotField.GetFilters method

Obtient tous les filtres de tableau croisé dynamique appliqués à ce champ de tableau croisé dynamique.

```csharp
public PivotFilter[] GetFilters()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFiltersDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["B1"].Value = "Sales";
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].Value = DateTime.Now.AddDays(i-2);
                worksheet.Cells[$"B{i}"].Value = i * 100;
            }

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B10", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Appliquer un filtre de date
            PivotField dateField = pivotTable.RowFields[0];
            DateTime startDate = DateTime.Now;
            DateTime endDate = DateTime.Now.AddDays(5);
            dateField.FilterByDate(PivotFilterType.DateBetween, startDate, endDate);
            
            // Obtenir et afficher les filtres
            PivotFilter[] filters = dateField.GetFilters();
            Console.WriteLine($"Number of filters applied: {filters.Length}");
            if (filters.Length > 0)
            {
                Console.WriteLine($"Filter type: {filters[0].FilterType}");
                Console.WriteLine($"Start date: {filters[0].GetDateTimeValues()[0]}");
                Console.WriteLine($"End date: {filters[0].GetDateTimeValues()[1]}");
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldGetFiltersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


