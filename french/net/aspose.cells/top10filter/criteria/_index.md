---
title: "Top10Filter.Criteria"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Top10Filter. La valeur réelle de la cellule dans la plage qui est utilisée pour effectuer la comparaison pour ce filtre. C'est la valeur en cache pendant le processus de rafraîchissement"
type: docs
url: /fr/net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

La valeur réelle de la cellule dans la plage qui est utilisée pour effectuer la comparaison pour ce filtre. C'est la valeur en cache pendant le processus de rafraîchissement.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### Remarques

NOTE: Ce membre est maintenant obsolète. À la place, veuillez ignorer cette propriété. Cette propriété sera supprimée 12 mois plus tard, à compter d'octobre 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class Top10FilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].PutValue(20 - i);
            }
            
            worksheet.AutoFilter.Range = "A1:A20";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Correction: accéder à la propriété Filter et la convertir en Top10Filter
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


