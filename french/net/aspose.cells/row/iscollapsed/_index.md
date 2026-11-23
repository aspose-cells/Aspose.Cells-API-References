---
title: "Row.IsCollapsed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. indique si la ligne est réduite"
type: docs
url: /fr/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

si la ligne est réduite

```csharp
public bool IsCollapsed { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer et styliser une ligne
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // Démontrer la propriété IsCollapsed
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Déplier la ligne
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Enregistrez le classeur
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


