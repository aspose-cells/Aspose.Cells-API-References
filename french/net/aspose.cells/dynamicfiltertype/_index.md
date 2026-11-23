---
title: "Énumération DynamicFilterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.DynamicFilterType. Type de filtre dynamique"
type: docs
url: /fr/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

Type de filtre dynamique.

```csharp
public enum DynamicFilterType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| AboveAverage | `0` | Affiche les valeurs supérieures à la moyenne. |
| BelowAverage | `1` | Affiche les valeurs inférieures à la moyenne. |
| LastMonth | `2` | Affiche les dates du mois dernier. |
| LastQuarter | `3` | Affiche les dates du dernier trimestre. |
| LastWeek | `4` | Affiche les dates de la semaine dernière. |
| LastYear | `5` | Affiche les dates de l'année dernière. |
| January | `6` | Affiche les dates de janvier, quelle que soit l'année. |
| October | `7` | Affiche les dates qui sont en octobre, quel que soit l'année. |
| November | `8` | Affiche les dates qui sont en novembre, quel que soit l'année. |
| December | `9` | Affiche les dates qui sont en décembre, quel que soit l'année. |
| February | `10` | Affiche les dates qui sont en février, quel que soit l'année. |
| March | `11` | Affiche les dates qui sont en mars, quel que soit l'année. |
| April | `12` | Affiche les dates qui sont en avril, quel que soit l'année. |
| May | `13` | Affiche les dates qui sont en mai, quel que soit l'année. |
| June | `14` | Affiche les dates qui sont en juin, quel que soit l'année. |
| July | `15` | Affiche les dates qui sont en juillet, quel que soit l'année. |
| August | `16` | Affiche les dates qui sont en août, quel que soit l'année. |
| September | `17` | Affiche les dates qui sont en septembre, quel que soit l'année. |
| NextMonth | `18` | Affiche les dates du mois prochain. |
| NextQuarter | `19` | Affiche les dates du trimestre prochain. |
| NextWeek | `20` | Affiche les dates de la semaine prochaine. |
| NextYear | `21` | Affiche les dates de l'année prochaine. |
| None | `22` | Aucun. |
| Quarter1 | `23` | Affiche les dates qui sont dans le 1er trimestre, quel que soit l'année. |
| Quarter2 | `24` | Affiche les dates qui sont dans le 2e trimestre, quel que soit l'année. |
| Quarter3 | `25` | Affiche les dates qui sont dans le 3e trimestre, quel que soit l'année. |
| Quarter4 | `26` | Affiche les dates qui sont dans le 4e trimestre, quel que soit l'année. |
| ThisMonth | `27` | Affiche les dates de ce mois. |
| ThisQuarter | `28` | Affiche les dates de ce trimestre. |
| ThisWeek | `29` | Affiche les dates de cette semaine. |
| ThisYear | `30` | Affiche les dates de cette année. |
| Today | `31` | Affiche les dates d'aujourd'hui. |
| Tomorrow | `32` | Affiche les dates de demain. |
| YearToDate | `33` | Affiche les dates entre le début de l'année et aujourd'hui, inclus. |
| Yesterday | `34` | Affiche les dates d'hier. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Appliquer le filtre automatique à la feuille de calcul
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Appliquer un filtre dynamique pour n'afficher que les dates de mars
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Enregistrez le classeur
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Afficher les résultats
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


