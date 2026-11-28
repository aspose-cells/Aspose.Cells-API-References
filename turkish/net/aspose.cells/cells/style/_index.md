---
title: "Cells.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Çalışma sayfasının varsayılan stilini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/style/
---
## Cells.Style property

Çalışma sayfasının varsayılan stilini alır ve ayarlar.

```csharp
public Style Style { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // A1 hücresine bir değer ayarlayın
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // Varsayılan stili alın ve biçimini değiştirin
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // Değiştirilen stili hücreye uygula
            cell.SetStyle(style);

            // Biçimlendirilmiş dize değerini gösterin
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


