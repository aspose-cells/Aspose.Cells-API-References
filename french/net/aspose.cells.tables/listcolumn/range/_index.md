---
title: "ListColumn.Range"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListColumn. Obtient la plage de ce ListColumn"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Obtient la plage de cette colonne de liste.

```csharp
public Range Range { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple pour créer un objet de liste
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // Créer un objet de liste
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // Obtenez le premier ListColumn
            ListColumn listCol = listObj.ListColumns[0];
            
            // Accédez à la plage du ListColumn
            Aspose.Cells.Range range = listCol.Range;
            
            // Affichez les informations de la plage
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // Modifiez les cellules dans la plage
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // Enregistrez le classeur
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


