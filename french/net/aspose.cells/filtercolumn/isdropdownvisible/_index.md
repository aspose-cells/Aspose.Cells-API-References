---
title: "FilterColumn.IsDropdownVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Indique si le bouton AutoFilter de cette colonne est visible"
type: docs
url: /fr/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

Indique si le bouton AutoFilter pour cette colonne est visible.

```csharp
public bool IsDropdownVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // Appliquer AutoFilter
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // Obtenir la colonne de filtre
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // Afficher la liste déroulante initialement
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // Masquer la liste déroulante
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // Enregistrez le classeur
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


