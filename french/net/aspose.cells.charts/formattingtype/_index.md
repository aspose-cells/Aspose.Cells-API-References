---
title: "Enum FormattingType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.FormattingType enum. Représente le type de formatage appliqué à un objet Area ou à un objet Line."
type: docs
url: /fr/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

Représente le type de formatage appliqué à un objet [`Area`](../../aspose.cells.drawing/area/) ou à un objet [`Line`](../../aspose.cells.drawing/line/).

```csharp
public enum FormattingType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Représente le type de formatage automatique. |
| Custom | `2` | Représente le type de formatage personnalisé. |
| None | `1` | Représente le type de formatage aucun. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // Instanciez un objet Workbook
            Workbook workbook = new Workbook();
            
            // Ajout d'une nouvelle feuille de calcul à l'objet Workbook
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Définition de la couleur de premier plan de la zone de tracé
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Définition de la couleur de premier plan de la zone du graphique
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // Définition de la couleur de premier plan de la zone du 1er NSeries
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // Définition de la couleur de premier plan de la zone du premier point NSeries
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Enregistrement du fichier Excel
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


