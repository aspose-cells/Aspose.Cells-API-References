---
title: "CalculationOptions.Recursive"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Bir hücreyi hesaplarken ve bu hücre diğer hücrelere bağlıyken bağımlı hücrelerin yinelemeli olarak hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Bir hücre hesaplanırken ve diğer hücrelere bağımlıysa bağımlı hücrelerin yinelemeli olarak hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'dur.

```csharp
public bool Recursive { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyRecursiveDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Dairesel referans oluştur
            cells["A1"].Formula = "=A2";
            cells["A2"].Formula = "=A1";

            // Recursive=true (varsayılan) ile ilk hesaplama
            CalculationOptions copts = new CalculationOptions();
            copts.Recursive = true;
            wb.CalculateFormula(copts);
            Console.WriteLine("Recursive calculation result (A2): " + cells["A2"].Value);

            // Recursive=false ile ikinci hesaplama
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine("Non-recursive calculation result (A2): " + cells["A2"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


