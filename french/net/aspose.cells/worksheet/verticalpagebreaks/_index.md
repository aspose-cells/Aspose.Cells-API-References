---
title: "Worksheet.VerticalPageBreaks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient la collection VerticalPageBreakCollection"
type: docs
url: /fr/net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Obtient la collection [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/).

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVerticalPageBreaksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Ajouter différents types de sauts de page verticaux
            verticalPageBreaks.Add(0, 10, 2);
            verticalPageBreaks.Add(4);
            verticalPageBreaks.Add(5, 3);
            verticalPageBreaks.Add("G5");

            // Supprimer un saut
            verticalPageBreaks.RemoveAt(1);

            // Imprimer les informations du saut
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"Break {i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


