---
title: "Sınıf CellRichValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellRichValue sınıfı. Hücrenin zengin değerini temsil eder"
type: docs
url: /tr/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Hücrenin zengin değerini temsil eder.

```csharp
public abstract class CellRichValue
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Görsel ile ilişkili alternatif metni alır. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Hücrenin hata değeri tipini alır. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Hücrenin görsel verisini alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine zengin bir değer ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // A1 hücresinden zengin değeri alın
            CellRichValue richValue = cell.GetRichValue();
            
            // Zengin değer özelliklerini göster
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Çalışma kitabını kaydedin
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


