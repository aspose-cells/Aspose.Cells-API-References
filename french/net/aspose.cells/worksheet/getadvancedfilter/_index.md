---
title: "Worksheet.GetAdvancedFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Obtient les paramètres du filtre avancé"
type: docs
url: /fr/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Obtient les paramètres du filtre avancé.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Configurer les données pour le filtrage
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // Configurer la plage de critères
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // Appliquer le filtre avancé
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // Obtenir le filtre avancé
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // Afficher les plages de filtre
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### Voir aussi

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


