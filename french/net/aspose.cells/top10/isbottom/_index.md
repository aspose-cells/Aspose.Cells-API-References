---
title: "Top10.IsBottom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Top10. Obtient ou définit si une règle top/bottom n est une règle bottom n. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/top10/isbottom/
---
## Top10.IsBottom property

Obtenir ou définir si une règle "top/bottom n" est une règle "bottom n". La valeur par défaut est false.

```csharp
public bool IsBottom { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyIsBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Ajouter une mise en forme conditionnelle
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            fcs.AddArea(new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 0 });

            // Ajouter la condition Top10
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Configurer les propriétés Top10
            Top10 top10 = fc.Top10;
            top10.IsBottom = true; // Highlight bottom values
            top10.IsPercent = false;
            top10.Rank = 3; // Highlight bottom 3 values

            workbook.Save("Top10IsBottomExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


