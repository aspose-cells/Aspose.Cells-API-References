---
title: "CellWatch.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellWatch. Obtient et définit la colonne de la cellule"
type: docs
url: /fr/net/aspose.cells/cellwatch/column/
---
## CellWatch.Column property

Obtient et définit la colonne de la cellule.

```csharp
public int Column { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];
            
            Console.WriteLine("Initial Column: " + cellWatch.Column);
            
            cellWatch.Column = 1;
            Console.WriteLine("Modified Column: " + cellWatch.Column);
            
            workbook.Save("CellWatchColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


