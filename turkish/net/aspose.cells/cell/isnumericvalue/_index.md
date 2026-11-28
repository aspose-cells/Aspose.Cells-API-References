---
title: "Cell.IsNumericValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin değerinin sayısal, tam sayı, çift ve tarih/zaman olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Bu hücrenin değerinin sayısal (int, double ve datetime) olup olmadığını gösterir

```csharp
public bool IsNumericValue { get; }
```

### Açıklamalar

Ayrıca hesaplanan sonucu kontrol etmek için formül hücresine de uygulanır

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsNumericValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere farklı veri türleri ekle
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue(123.45); // Numeric value

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Hello World"); // String value

            // Hücrelerin sayısal değerler içerip içermediğini kontrol edin
            Console.WriteLine("Cell A1 IsNumericValue: " + cell1.IsNumericValue);
            Console.WriteLine("Cell A2 IsNumericValue: " + cell2.IsNumericValue);

            // Koşullu mantıkla kullanımını gösterin
            if (cell1.IsNumericValue)
            {
                Console.WriteLine("Cell A1 contains a numeric value: " + cell1.DoubleValue);
            }

            if (!cell2.IsNumericValue)
            {
                Console.WriteLine("Cell A2 does not contain a numeric value");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


