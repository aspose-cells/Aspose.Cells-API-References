---
title: "Cell.GetTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient le tableau qui contient cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/gettable/
---
## Cell.GetTable method

Obtient le tableau qui contient cette cellule.

```csharp
public ListObject GetTable()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellMethodGetTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créez un tableau avec des en-têtes et des données
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Créez un ListObject (tableau) à partir de la plage de données
            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Démontrez la méthode GetTable
            Cell cellInTable = cells["B2"];
            ListObject resultTable = cellInTable.GetTable();
            
            Console.WriteLine("Table found: " + (resultTable != null));
            Console.WriteLine("Table range: " + resultTable.StartRow + "," + resultTable.StartColumn + 
                            " to " + resultTable.EndRow + "," + resultTable.EndColumn);
        }
    }
}
```

### Voir aussi

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


