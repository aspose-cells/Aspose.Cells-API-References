---
title: "AutoFilter.FilterColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFilter. Obtient la collection des colonnes de filtre"
type: docs
url: /fr/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Obtient la collection des colonnes de filtre.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // Appliquer le filtre automatique
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // Filtrer la colonne 2 (Status) pour les valeurs "Present"
            autoFilter.Filter(2, "Present");
            
            // Accéder à la colonne de filtre
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // Enregistrez le classeur
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


