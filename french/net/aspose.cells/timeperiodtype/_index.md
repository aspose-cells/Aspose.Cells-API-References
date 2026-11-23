---
title: "Enum TimePeriodType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.TimePeriodType enum. Utilisé dans une règle de mise en forme conditionnelle FormatConditionType.TimePeriod. Ce sont des périodes de temps dynamiques qui changent en fonction de la date à laquelle la mise en forme conditionnelle est actualisée / appliquée."
type: docs
url: /fr/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

Utilisé dans une règle de mise en forme conditionnelle FormatConditionType.TimePeriod. Ce sont des périodes temporelles dynamiques, qui changent en fonction de la date à laquelle la mise en forme conditionnelle est actualisée/appliquée.

```csharp
public enum TimePeriodType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Today | `0` | Date d'aujourd'hui. |
| Yesterday | `1` | Date d'hier. |
| Tomorrow | `2` | Date de demain. |
| Last7Days | `3` | Une date parmi les sept derniers jours. |
| ThisMonth | `4` | Une date se produisant dans ce mois calendaire. |
| LastMonth | `5` | Une date se produisant le mois civil précédent. |
| NextMonth | `6` | Une date se produisant le mois civil suivant. |
| ThisWeek | `7` | Une date se produisant cette semaine. |
| LastWeek | `8` | Une date se produisant la semaine dernière. |
| NextWeek | `9` | Une date se produisant la semaine prochaine. |
| ThisYear | `10` | Une date se produisant cette année. Seulement pour .ods. |
| LastYear | `11` | Une date se produisant l'année dernière. Seulement pour .ods. |
| NextYear | `12` | Une date se produisant l'année prochaine. Seulement pour .ods. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une règle de mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définir la zone de cellules pour la mise en forme conditionnelle
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Ajouter une condition pour la période de temps
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Définir le type de période de temps
            fc.TimePeriod = TimePeriodType.Today;

            // Enregistrez le classeur
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


