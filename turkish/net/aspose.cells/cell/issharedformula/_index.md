---
title: "Cell.IsSharedFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücre formülünün paylaşılan formülün bir parçası olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Hücre formülünün paylaşılan bir formülün parçası olup olmadığını gösterir.

```csharp
public bool IsSharedFormula { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralıkta paylaşılan formülü ayarla
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // Hücrelerin paylaşılan formül içerip içermediğini kontrol et
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


