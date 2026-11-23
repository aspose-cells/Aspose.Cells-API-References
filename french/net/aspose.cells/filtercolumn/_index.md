---
title: "Classe FilterColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FilterColumn. Représente un filtre pour une seule colonne ou une colonne du tableau"
type: docs
url: /fr/net/aspose.cells/filtercolumn/
---
## FilterColumn class

Représente un filtre pour une seule colonne ou une colonne du tableau.

```csharp
public class FilterColumn
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | Obtient [`ColorFilter`](../colorfilter/) pour filtrer les données par couleur. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | Obtient [`CustomFilterCollection`](../customfiltercollection/) pour filtrer les données selon des critères personnalisés. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | Obtient [`DynamicFilter`](./dynamicfilter/) pour filtrer avec des critères dynamiques. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Obtient et définit le décalage de colonne dans la plage. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsolete.**) Obtient et définit la condition du filtrage des données. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Obtient et définit le type du filtrage des données. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | Obtient [`FilterValueCollection`](../filtervaluecollection/) pour filtrer les données par libellés ou date/heure. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | Obtient [`IconFilter`](./iconfilter/) pour filtrer les données par icône. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Indique si le bouton AutoFilter pour cette colonne est visible. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Obsolete.**) Obtient [`MultipleFilterCollection`](../multiplefiltercollection/) pour filtrer les données par libellés ou date/heure. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | Obtient [`Top10Filter`](./top10filter/) pour filtrer les données par rang. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | Sélectionne tout. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;

namespace AsposeCellsExamples
{
    public class FilterColumnDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // Appliquer le filtre automatique à la plage
            sheet.AutoFilter.SetRange(0, 0, 3);

            // Ajouter un filtre à la première colonne (Nom)
            sheet.AutoFilter.AddFilter(0, "John");

            // Ajouter un filtre à la deuxième colonne (Âge)
            sheet.AutoFilter.AddFilter(1, "30");

            // Actualiser le filtre pour l'appliquer
            sheet.AutoFilter.Refresh();

            // Accéder à la collection FilterColumnCollection
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Accéder à la première FilterColumn
            FilterColumn filterColumn = filterColumns[0];

            // Afficher les propriétés de la FilterColumn
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // Enregistrez le classeur
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


