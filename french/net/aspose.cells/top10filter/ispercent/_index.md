---
title: "Top10Filter.IsPercent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Top10Filter. Indique s'il faut filtrer ou non par valeur en pourcentage de la colonne"
type: docs
url: /fr/net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Indique s'il faut filtrer ou non par la valeur en pourcentage de la colonne

```csharp
public bool IsPercent { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Appliquer le filtre top 10 (pas en pourcentage)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Obtenir le filtre et démontrer la propriété IsPercent
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // Appliquer le filtre top 10 en pourcentage
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### Voir aussi

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


