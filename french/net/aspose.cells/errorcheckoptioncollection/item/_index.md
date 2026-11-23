---
title: "ErrorCheckOptionCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ErrorCheckOptionCollection. Obtient l'objet ErrorCheckOption par l'index donné"
type: docs
url: /fr/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Obtient l'objet [`ErrorCheckOption`](../../errorcheckoption/) par l'index donné.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index |

### Valeur de retour

Retourne l'objet [`ErrorCheckOption`](../../errorcheckoption/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;
            int optionIdx = opts.Add();
            
            // Démontrer l'utilisation de la propriété Item
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


