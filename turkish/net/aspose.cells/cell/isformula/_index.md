---
title: "Cell.IsFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Belirtilen hücrenin formül içerip içermediğini temsil eder"
type: docs
url: /tr/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Belirtilen hücrenin formül içerip içermediğini temsil eder.

```csharp
public bool IsFormula { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine formül ekle
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // A2 hücresine düz değer ekle
            worksheet.Cells["A2"].PutValue("Test");
            
            // Hücrelerin formül içerip içermediğini kontrol et
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


