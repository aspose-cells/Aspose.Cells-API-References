---
title: "Énumération DataLabelsSeparatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Charts.DataLabelsSeparatorType. Représente le type de séparateur des étiquettes de données"
type: docs
url: /fr/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

Représente le type de séparateur des étiquettes de données.

```csharp
public enum DataLabelsSeparatorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Auto | `0` | Représente le séparateur automatique |
| Space | `1` | Représente l'espace(" ") |
| Comma | `2` | Représente la virgule(",") |
| Semicolon | `3` | Représente le point-virgule(";") |
| Period | `4` | Représente le point(".") |
| NewLine | `5` | Représente le saut de ligne("\n") |
| Custom | `6` | Représente un séparateur personnalisé |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données pour le graphique
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez la série de données au graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez aux étiquettes de données de la première série
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Définir le type de séparateur sur la virgule
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // Activer les étiquettes de données et définir certaines propriétés
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // Définir les propriétés de la police
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // Enregistrez le classeur
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


