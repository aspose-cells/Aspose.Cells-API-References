---
title: "Top10.Rank"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Top10. Obtient ou définit la valeur de n dans une règle de mise en forme conditionnelle top/bottom n. Si IsPercent est vrai, la valeur doit être comprise entre 0 et 100. Sinon, elle doit être comprise entre 0 et 1000. La valeur par défaut est 10."
type: docs
url: /fr/net/aspose.cells/top10/rank/
---
## Top10.Rank property

Obtenir ou définir la valeur de "n" dans une règle de mise en forme conditionnelle "top/bottom n". Si IsPercent est true, la valeur doit être comprise entre 0 et 100. Sinon, elle doit être comprise entre 0 et 1000. La valeur par défaut est 10.

```csharp
public int Rank { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class Top10PropertyRankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            Top10 top10 = fc.Top10;
            top10.Rank = 5;

            workbook.Save("Top10RankExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Top10](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


