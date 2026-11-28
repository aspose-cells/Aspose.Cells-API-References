---
title: "CellValue.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellValue özelliği. Hücre değerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Hücre değerini alır veya ayarlar.

```csharp
public object Value { get; set; }
```

### Açıklamalar

Değer, [`Type`](../type/) ile eşleşen doğru nesne türünde olmalıdır:

| **Type** | **Value** |
| --- | --- |
| IsNull | null, diğer tüm nesneler yok sayılacak |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | hata dizesi, örneğin "#VALUE!", "#NAME?", ... |

### Örnekler

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

### Ayrıca Bakınız

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


