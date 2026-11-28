---
title: "Cells.IsBlankColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Verilen sütunun boş olup veri içermediğini kontrol eder"
type: docs
url: /tr/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Verilen sütunun boş olup olmadığını kontrol eder (herhangi bir veri içermez).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | sütun indeksi |

### Dönüş Değeri

verilen sütun veri içermiyorsa true

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sütun 2'nin boş olup olmadığını kontrol et (yeni çalışma sayfası için true olmalı)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // Sütun 2'ye veri ekle
            worksheet.Cells["B1"].PutValue("Test Data");

            // Tekrar kontrol et (artık false olmalı)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // Tamamen boş sütunlarla başka bir çalışma sayfası oluştur
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // Boş çalışma sayfasındaki bir sütunu kontrol et (true olmalı)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


