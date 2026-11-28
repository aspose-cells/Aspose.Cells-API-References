---
title: "Cell.IsArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücre formülünün bir dizi formülü olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Hücre formülünün bir dizi formülü olup olmadığını gösterir.

```csharp
public bool IsArrayFormula { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B2 hücresinde bir dizi formülü oluştur
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // Hücrenin bir dizi formülü içerip içermediğini kontrol et
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // Çalışma kitabını kaydedin
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


