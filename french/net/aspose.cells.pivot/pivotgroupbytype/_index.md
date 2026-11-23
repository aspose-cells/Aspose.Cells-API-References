---
title: "Énumération PivotGroupByType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Pivot.PivotGroupByType. Représente le type de regroupement"
type: docs
url: /fr/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

Représente le type de regroupement.

```csharp
[Flags]
public enum PivotGroupByType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| RangeOfValues | `1` | Regrouper par nombres. |
| Numbers | `1` | Regrouper par nombres. |
| Seconds | `2` | Présente le type de regroupement par secondes. |
| Minutes | `4` | Présente le type de regroupement par minutes. |
| Hours | `8` | Présente le type de regroupement par heures. |
| Days | `10` | Présente le type de regroupement par jours. |
| Months | `20` | Présente le type de regroupement par mois. |
| Quarters | `40` | Présente le type de regroupement par trimestres. |
| Years | `80` | Présente le type de regroupement par années. |
| DateTimes | `FE` | Présente tous les types de regroupement des dates et heures. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);

            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);

            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Accédez aux paramètres du groupe
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Générer les paramètres du groupe
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Enregistrez le classeur
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


