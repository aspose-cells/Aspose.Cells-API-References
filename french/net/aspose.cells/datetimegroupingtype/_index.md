---
title: "Enum DateTimeGroupingType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DateTimeGroupingType enum. Spécifie comment regrouper les valeurs dateTime"
type: docs
url: /fr/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

Spécifie comment regrouper les valeurs dateTime.

```csharp
public enum DateTimeGroupingType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Day | `0` | Regrouper par jour. |
| Hour | `1` | Regrouper par heure. |
| Minute | `2` | Regrouper par minute. |
| Month | `3` | Regrouper par mois. |
| Second | `4` | Regrouper par seconde. |
| Year | `5` | Regrouper par année. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // Création d'un classeur et accès à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout de données d'exemple
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // Création d'un AutoFilter et définition de la plage
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // Ajout de filtres de date avec différents DateTimeGroupingType
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // Enregistrement du classeur
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


