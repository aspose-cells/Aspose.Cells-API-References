---
title: "CellsHelper.ColumnNameToIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Obtient l'index de colonne selon le nom de la colonne"
type: docs
url: /fr/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Obtient l'indice de colonne selon le nom de la colonne.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnName | String | Nom de colonne. |

### Valeur de retour

Index de colonne.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnNameToIndexWithStringDemo
    {
        public static void Run()
        {
            int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
            string columnName = CellsHelper.ColumnIndexToName(columnIndex);
            
            Console.WriteLine("Column Name: " + columnName);
            Console.WriteLine("Column Index: " + columnIndex);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


