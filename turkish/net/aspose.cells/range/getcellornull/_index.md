---
title: "Range.GetCellOrNull"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Bu aralıkta Cell nesnesini veya null değerini alır"
type: docs
url: /tr/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

Bu aralıkta [`Cell`](../../cell/) nesnesini veya null değerini alır.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | Int32 | Bu aralıktaki satır ofseti, sıfır tabanlı. |
| columnOffset | Int32 | Bu aralıktaki sütun ofseti, sıfır tabanlı. |

### Dönüş Değeri

[`Cell`](../../cell/) object.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık oluşturun
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // Aralığı bazı verilerle doldurun
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // Int32 parametreleriyle GetCellOrNull yöntemini gösterin
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // Aralık dışındaki bir hücre almaya çalışın (null döndürmelidir)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


