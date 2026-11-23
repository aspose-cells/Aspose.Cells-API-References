---
title: "Cells.CheckRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l'élément Row ou null à l'index de ligne de cellule spécifié"
type: docs
url: /fr/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Obtient l'élément [`Row`](../../row/) ou null à l'index de ligne de cellule spécifié.

```csharp
public Row CheckRow(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne |

### Valeur de retour

Renvoie l'objet [`Row`](../../row/) si l'objet ligne existe, sinon renvoie null.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckRowWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Remplissez quelques données
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // Vérifier si la ligne existe et obtenir l'objet ligne
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // Vérifier une ligne inexistante
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### Voir aussi

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


