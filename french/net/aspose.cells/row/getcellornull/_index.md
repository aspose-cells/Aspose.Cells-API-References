---
title: "Row.GetCellOrNull"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Obtient la cellule ou null à l'indice spécifique"
type: docs
url: /fr/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Obtient la cellule ou null à l'index spécifié.

```csharp
public Cell GetCellOrNull(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | L'index de colonne |

### Valeur de retour

Renvoie l'objet cellule si la cellule existe. Ou renvoie null si l'objet cellule n'existe pas.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Ajoutez des données d'exemple
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // Obtenir la première ligne
            Row row = ws.Cells.Rows[0];

            // Démontrer GetCellOrNull avec le paramètre Int32
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


