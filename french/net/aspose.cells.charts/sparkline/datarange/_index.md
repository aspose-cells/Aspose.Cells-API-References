---
title: "Sparkline.DataRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Sparkline. Représente la plage de données du sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparkline/datarange/
---
## Sparkline.DataRange property

Représente la plage de données du sparkline.

```csharp
public string DataRange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyDataRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(7);
            sheet.Cells["A4"].PutValue(2);
            sheet.Cells["A5"].PutValue(9);

            // Ajouter un groupe de sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A5", false, new CellArea { StartRow = 0, StartColumn = 1, EndRow = 0, EndColumn = 1 });
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Accédez au premier sparkline et affichez sa plage de données
            Sparkline sparkline = group.Sparklines[0];
            Console.WriteLine("Sparkline DataRange: " + sparkline.DataRange);
        }
    }
}
```

### Voir aussi

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


