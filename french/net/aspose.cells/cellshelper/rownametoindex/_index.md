---
title: "CellsHelper.RowNameToIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Obtient l'index de ligne selon le nom de ligne"
type: docs
url: /fr/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Obtient l'indice de ligne selon le nom de la ligne.

```csharp
public static int RowNameToIndex(string rowName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowName | String | Nom de ligne. |

### Valeur de retour

Index de ligne.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowNameToIndexWithStringDemo
    {
        public static void Run()
        {
            string rowName = "11";
            int rowIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name '{0}' converted to index: {1}", rowName, rowIndex);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


