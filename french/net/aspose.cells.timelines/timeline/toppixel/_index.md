---
title: "Timeline.TopPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Timeline. Retourne ou définit le décalage vertical de la forme de la chronologie par rapport à sa ligne supérieure en pixels"
type: docs
url: /fr/net/aspose.cells.timelines/timeline/toppixel/
---
## Timeline.TopPixel property

Retourne ou définit le décalage vertical de la forme de la chronologie par rapport à sa ligne supérieure, en pixels.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Remarques

REMARQUE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Top. Cette propriété sera supprimée 12 mois plus tard, à compter de mai 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyTopPixelDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplissez des données d'exemple
            cells["A1"].Value = "Date";
            cells["A2"].Value = new DateTime(2023, 1, 1);
            cells["A3"].Value = new DateTime(2023, 2, 1);
            cells["A4"].Value = new DateTime(2023, 3, 1);
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Ajouter PivotTable
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Ajouter Timeline
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];

            // Définir les propriétés de Timeline, y compris TopPixel
            timeline.TopPixel = 50;
            timeline.HeightPixel = 100;
            timeline.WidthPixel = 300;

            // Enregistrez le classeur
            book.Save("TimelineTopPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


