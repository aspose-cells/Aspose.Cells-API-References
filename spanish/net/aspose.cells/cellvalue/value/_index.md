---
title: "CellValue.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellValue. Obtiene o establece el valor de la celda"
type: docs
url: /es/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Obtiene o establece el valor de la celda.

```csharp
public object Value { get; set; }
```

### Observaciones

El valor debe ser del tipo de objeto correcto que corresponde a [`Type`](../type/):

| **Type** | **Value** |
| --- | --- |
| IsNull | null, cualquier otro objeto será ignorado |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | cadena de error como "#VALUE!", "#NAME?", ... |

### Ejemplos

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

### Ver también

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


