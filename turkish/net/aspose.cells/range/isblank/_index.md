---
title: "Range.IsBlank"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Aralığın değer içerip içermediğini gösterir"
type: docs
url: /tr/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Aralığın değer içerip içermediğini gösterir.

```csharp
public bool IsBlank()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bir aralık oluştur ve boş olup olmadığını kontrol et (doğru olmalı)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // Bir hücreye bir değer koy ve tekrar kontrol et (yanlış olmalı)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


