---
title: "Énum Bar3DShapeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énum Aspose.Cells.Charts.Bar3DShapeType. Représente la forme utilisée avec le graphique à barres ou colonnes 3D"
type: docs
url: /fr/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

Représente la forme utilisée avec le graphique à barres ou colonnes 3D.

```csharp
public enum Bar3DShapeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Box | `0` | Boîte |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cylindre |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class Bar3DShapeTypeDemo
    {
        public static void Bar3DShapeTypeExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            // Ajout d'une nouvelle feuille de calcul à l'objet Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];
            // Ajoute NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Définir la source de données pour les données de catégorie de NSeries
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // Définir les valeurs de la série
            series.Values = "=B1:B4";

            // Définir le type de forme 3D pour la série
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Enregistrement du fichier Excel
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // Définir le type de forme 3D pour la série
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // Enregistrement du fichier Excel
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


