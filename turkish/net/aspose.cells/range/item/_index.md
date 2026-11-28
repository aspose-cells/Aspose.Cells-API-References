---
title: "Range.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range özelliği. Bu aralıktaki Cell nesnesini alır"
type: docs
url: /tr/net/aspose.cells/range/item/
---
## Range indexer

Bu aralıktaki [`Cell`](../../cell/) nesnesini alır.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| rowOffset | Bu aralıktaki satır ofseti, sıfır tabanlı. |
| columnOffset | Bu aralıktaki sütun ofseti, sıfır tabanlı. |

### Dönüş Değeri

[`Cell`](../../cell/) object.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangePropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri oluştur
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // Bir aralık oluşturun ve Item özelliğini gösterin
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // Item özelliğini kullanarak başlıkları ayarlayın
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // Item özelliğini kullanarak verileri doldurun
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // Item özelliğini kullanarak başlık satırını biçimlendirin
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


