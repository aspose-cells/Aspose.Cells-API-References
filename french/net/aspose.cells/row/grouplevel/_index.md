---
title: "Row.GroupLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient le niveau de groupe de la ligne"
type: docs
url: /fr/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Obtient le niveau de groupe de la ligne.

```csharp
public byte GroupLevel { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grouper les lignes 4-6 (caché = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // Accéder au niveau de groupe de la ligne 4
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // Dégrouper les lignes
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


