---
title: "Enum CategoryType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.CategoryType enum. Représente le type d'axe de catégorie"
type: docs
url: /fr/net/aspose.cells.charts/categorytype/
---
## CategoryType enumeration

Représente le type d'axe de catégorie.

```csharp
public enum CategoryType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CategoryTypeDemo
    {
        public static void CategoryTypeExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            // Ajout d'une nouvelle feuille de calcul à l'objet Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Dates");
            worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells["B1"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(30);

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];
            // Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("B2:C4", true);

            // Définition des noms de catégorie pour l'axe X à partir de la plage "A2:A5"
            chart.NSeries[0].XValues = "A2:A4";

            // Définition du type d'axe de catégorie sur TimeScale
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // Définition de l'échelle de l'unité principale pour l'axe de catégorie
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // Définition de l'échelle de l'unité secondaire pour l'axe de catégorie
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Enregistrement du fichier Excel
            workbook.Save("CategoryTypeExample.xlsx");
            workbook.Save("CategoryTypeExample.pdf");

        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


