---
title: "ListObject.EndRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Obtient la ligne de fin de la plage"
type: docs
url: /fr/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Obtient la ligne de fin de la plage.

```csharp
public int EndRow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Créer des données d'exemple
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // Créer un objet de liste/table
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // Afficher la ligne de fin initiale
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // Ajouter une nouvelle ligne au tableau
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // Afficher la ligne de fin mise à jour
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // Enregistrez le classeur
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


