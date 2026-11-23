---
title: "ListColumn.Formula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListColumn. Obtient et définit la formule du ListColumn"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Obtient et définit la formule de la colonne de liste.

```csharp
public string Formula { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créez des données d'exemple et un tableau
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["A3"].PutValue(10);
            sheet.Cells["A4"].PutValue(15);
            
            sheet.Cells["B1"].PutValue("Doubled");
            sheet.Cells["B2"].PutValue("=A2*2");
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            
            // Ajoutez une formule au ListColumn
            ListColumn column = table.ListColumns[0];
            column.Formula = "=A2*3"; // This will apply to all cells in the column
            
            // Enregistrez le classeur
            workbook.Save("ListColumnFormulaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


