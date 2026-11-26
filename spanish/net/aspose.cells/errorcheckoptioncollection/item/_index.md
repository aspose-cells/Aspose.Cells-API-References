---
title: "ErrorCheckOptionCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ErrorCheckOptionCollection. Obtiene el objeto ErrorCheckOption por el índice dado"
type: docs
url: /es/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Obtiene el objeto [`ErrorCheckOption`](../../errorcheckoption/) por el índice dado.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice |

### Valor de retorno

Devuelve el objeto [`ErrorCheckOption`](../../errorcheckoption/)

### Ejemplos

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
            
            // Demostrar el uso de la propiedad Item
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


