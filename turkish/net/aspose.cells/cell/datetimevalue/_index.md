---
title: "Cell.DateTimeValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell property. Hücrede bulunan DateTime değerini alır."
type: docs
url: /tr/net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Hücrede bulunan DateTime değerini alır.

```csharp
public DateTime DateTimeValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDateTimeValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // A1 hücresine bir DateTime değeri ayarla
            DateTime testDate = new DateTime(2023, 12, 25);
            cells["A1"].PutValue(testDate);

            // Hücreyi tarihi gösterecek şekilde biçimlendir
            Style style = cells["A1"].GetStyle();
            style.Custom = "yyyy-MM-dd";
            cells["A1"].SetStyle(style);

            // DateTimeValue değerini al ve doğrula
            DateTime retrievedDate = cells["A1"].DateTimeValue;
            Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
            Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));

            // B1 hücresine başka bir DateTime değeri ayarla
            DateTime anotherDate = new DateTime(2024, 1, 1);
            cells["B1"].PutValue(anotherDate);

            // B1'den DateTimeValue değerini göster
            Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


