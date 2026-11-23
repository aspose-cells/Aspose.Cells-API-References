---
title: "FilterColumn.FieldIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient et définit le décalage de colonne dans la plage"
type: docs
url: /fr/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

Obtient et définit le décalage de colonne dans la plage.

```csharp
public int FieldIndex { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:B4";
            
            // Ajouter un filtre à la première colonne (Department)
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // Obtenir la colonne de filtre
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // Démontrer la propriété FieldIndex
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // Rafraîchir et enregistrer
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


