---
title: "Timeline.LeftPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Timeline. Retourne ou définit le décalage horizontal de la forme de la chronologie depuis sa colonne de gauche en pixels"
type: docs
url: /fr/net/aspose.cells.timelines/timeline/leftpixel/
---
## Timeline.LeftPixel property

Retourne ou définit le décalage horizontal de la forme de la chronologie, en pixels.

```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Left. Cette propriété sera supprimée 12 mois après mai 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyLeftPixelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();

            // Ajoutez le Timeline et récupérez‑le depuis la collection
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Démontrez la propriété LeftPixel
            timeline.LeftPixel = 150;
            timeline.TopPixel = 50;
            timeline.WidthPixel = 200;
            timeline.HeightPixel = 80;

            // Enregistrer le classeur
            workbook.Save("TimelineLeftPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


