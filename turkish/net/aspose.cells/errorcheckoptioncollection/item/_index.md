---
title: "ErrorCheckOptionCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ErrorCheckOptionCollection özelliği. Verilen indeks ile ErrorCheckOption nesnesini alır"
type: docs
url: /tr/net/aspose.cells/errorcheckoptioncollection/item/
---
## ErrorCheckOptionCollection indexer

Verilen indeks ile [`ErrorCheckOption`](../../errorcheckoption/) nesnesini alır.

```csharp
public ErrorCheckOption this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks |

### Dönüş Değeri

[`ErrorCheckOption`](../../errorcheckoption/) nesnesini döndür

### Örnekler

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
            
            // Item özelliğinin kullanımını göster
            ErrorCheckOption opt = opts[optionIdx];
            
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.AddRange(CellArea.CreateCellArea("A1", "B3"));

            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ErrorCheckOption](../../errorcheckoption/)
* class [ErrorCheckOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


