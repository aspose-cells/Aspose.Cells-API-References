---
title: "Classe Top10Filter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Top10Filter. Représente les N pour cent supérieurs ou le nombre d'éléments à filtrer"
type: docs
url: /fr/net/aspose.cells/top10filter/
---
## Top10Filter class

Représente le top N (pourcentage ou nombre d'éléments) à filtrer.

```csharp
public class Top10Filter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) La valeur réelle de la cellule dans la plage qui est utilisée pour effectuer la comparaison pour ce filtre. C’est la valeur du cache pendant le processus de rafraîchissement. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Indique s'il faut filtrer ou non par la valeur en pourcentage de la colonne |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Indique s'il faut filtrer ou non par ordre supérieur |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Obtient et définit la valeur supérieure ou inférieure à utiliser comme critère de filtrage. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Appliquez le filtre automatique et le filtre top 10
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Obtenez le Top10Filter et vérifiez ses propriétés
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Rafraîchissez le filtre et vérifiez les lignes masquées
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Enregistrez le classeur
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


