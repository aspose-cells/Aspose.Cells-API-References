---
title: "Cell.IsDynamicArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrenin formülünün dinamik dizi formülü (true) veya eski dizi formülü (false) olduğunu gösterir."
type: docs
url: /tr/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Hücrenin formülünün dinamik dizi formülü (true) mı yoksa eski dizi formülü (false) mı olduğunu gösterir.

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine dinamik dizi formülü ayarla.
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // Hücrenin dinamik dizi formülü içerip içermediğini kontrol et.
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // Çalışma kitabını kaydedin
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


