---
title: "Cell.ToJson"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Cell'i JSON yapı verisine dönüştür"
type: docs
url: /tr/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

[`Cell`](../) öğesini JSON yapı verisine dönüştür.

```csharp
public string ToJson()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek verileri ve stilleri ayarla
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // Hücreyi al ve JSON'a dönüştür
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // JSON'ı çıktı olarak ver
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


