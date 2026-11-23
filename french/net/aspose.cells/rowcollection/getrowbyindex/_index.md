---
title: "RowCollection.GetRowByIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode RowCollection. Obtient l'objet ligne selon la position dans la liste"
type: docs
url: /fr/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

Obtient l'objet ligne par sa position dans la liste.

```csharp
public Row GetRowByIndex(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | La position. |

### Valeur de retour

L'objet Row à la position donnée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetRowByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtenir la ligne par index (base 0)
            Row row = sheet.Cells.Rows.GetRowByIndex(0);
            
            if (row == null)
            {
                Console.WriteLine("Row at index 0 is null (not created yet)");
            }
            else
            {
                Console.WriteLine("Row at index 0 exists");
            }
        }
    }
}
```

### Voir aussi

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


