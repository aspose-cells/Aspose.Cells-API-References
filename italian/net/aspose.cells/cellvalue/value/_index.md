---
title: "CellValue.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellValue. Ottiene o imposta il valore della cella"
type: docs
url: /it/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Ottiene o imposta il valore della cella.

```csharp
public object Value { get; set; }
```

### Osservazioni

Il valore deve essere del tipo corretto di oggetto corrispondente a [`Type`](../type/):

| **Type** | **Valore** |
| --- | --- |
| IsNull | null, qualsiasi altro oggetto verrà ignorato |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | stringa di errore come "#VALUE!", "#NAME?", ... |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            worksheet.Cells["A1"].PutValue(cellValue.Value);

            workbook.Save("CellValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


