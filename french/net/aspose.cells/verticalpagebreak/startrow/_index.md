---
title: "VerticalPageBreak.StartRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VerticalPageBreak. Obtient l'index de ligne de début du saut de page vertical"
type: docs
url: /fr/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Obtient l'index de ligne de début du saut de page vertical.

```csharp
public int StartRow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des sauts de page verticaux avec la ligne de début souhaitée (2) initialement
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // Afficher la propriété StartRow
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Comme StartRow est en lecture seule, nous devons le supprimer et le réajouter pour le modifier
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Enregistrez le classeur
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


