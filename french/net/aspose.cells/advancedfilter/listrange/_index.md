---
title: "AdvancedFilter.ListRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AdvancedFilter. Obtient la plage de liste de ce filtre avancé"
type: docs
url: /fr/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Obtient la plage de la liste de ce filtre avancé.

```csharp
public string ListRange { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Remplissez des données d'exemple
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // Configurer le filtre avancé
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange est en lecture seule et est définie automatiquement lors de la création du filtre
            // Nous ne pouvons que le lire, pas le définir directement
            
            // Afficher la plage de liste (affichera la plage déterminée automatiquement)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // Enregistrez le classeur
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


