---
title: "CellValue.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellValue. Получает или задаёт значение ячейки"
type: docs
url: /ru/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

Получает или задает значение ячейки.

```csharp
public object Value { get; set; }
```

### Примечания

Значение должно быть объектом правильного типа, соответствующего [`Type`](../type/):

| **Type** | **Value** |
| --- | --- |
| IsNull | null, любой другой объект будет игнорироваться |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | строка ошибки, например "#VALUE!", "#NAME?", ... |

### Примеры

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

### См. также

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


