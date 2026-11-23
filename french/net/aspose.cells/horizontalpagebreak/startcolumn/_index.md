---
title: "HorizontalPageBreak.StartColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HorizontalPageBreak. Obtient l'index de la colonne de début de cette rupture de page horizontale"
type: docs
url: /fr/net/aspose.cells/horizontalpagebreak/startcolumn/
---
## HorizontalPageBreak.StartColumn property

Obtient l'indice de colonne de début de ce saut de page horizontal.

```csharp
public int StartColumn { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyStartColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des ruptures de page à différentes colonnes pour démontrer StartColumn
            int index1 = worksheet.HorizontalPageBreaks.Add("Y30");
            int index2 = worksheet.HorizontalPageBreaks.Add("B30");
            
            HorizontalPageBreak hPageBreak1 = worksheet.HorizontalPageBreaks[index1];
            HorizontalPageBreak hPageBreak2 = worksheet.HorizontalPageBreaks[index2];
            
            Console.WriteLine($"First Break Start Column: {hPageBreak1.StartColumn}");
            Console.WriteLine($"Second Break Start Column: {hPageBreak2.StartColumn}");
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


