---
title: "Cell.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrede bulunan değeri alır/ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/value/
---
## Cell.Value property

Bu hücrede bulunan değeri alır/ayarlar.

```csharp
public object Value { get; set; }
```

### Açıklamalar

Olası tip:

null,

Boolean,

DateTime,

Double,

Integer

String.

int değeri için, bir Integer nesnesi veya bir Double nesnesi olarak döndürülebilir. Ve döndürülen değerin her zaman aynı nesne türünde tutulacağına dair bir garanti yoktur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Değerleri Value özelliğini kullanarak ayarlayın
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // null değerleri gösterin
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // Değerleri görüntüleyin
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


