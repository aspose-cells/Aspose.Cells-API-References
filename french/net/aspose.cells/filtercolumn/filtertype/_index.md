---
title: "FilterColumn.FilterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient et définit le type de filtrage des données"
type: docs
url: /fr/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Obtient et définit le type du filtrage des données.

```csharp
public FilterType FilterType { get; set; }
```

### Remarques

L'objet de filtre correspondant sera créé lorsque cette propriété est définie et la propriété correspondante doit être utilisée pour obtenir l'objet de filtre en conséquence:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // Appliquer un filtre automatique en utilisant une plage de chaînes
            sheet.AutoFilter.Range = "A1:B4";

            // Ajouter différents types de filtres pour démontrer la propriété FilterType
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // Obtenir les colonnes de filtre
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Afficher le FilterType pour chaque colonne
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // Enregistrez le classeur
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


