---
title: "CalculationOptions.CalcStackSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Hücreleri özyinelemeli olarak hesaplamak için yığın boyutu. Varsayılan değer 200."
type: docs
url: /tr/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

Hücreleri özyinelemeli olarak hesaplamak için yığın boyutu. Varsayılan değer 200.

```csharp
public int CalcStackSize { get; set; }
```

### Açıklamalar

Bağımlılık ağacında özyinelemeli olarak hesaplanması gereken çok sayıda hücre olduğunda, hesaplama sürecinde StackOverflowException oluşabilir. Bu durumda, kullanıcı bu özellik için daha küçük bir değer belirtmelidir. Böyle bir durumda, kullanıcı bu özelliğin uygun değerini gerçek formüller ve verilere göre belirlemelidir. Ancak, çok küçük bir değer formül hesaplamasının performansını düşürebilir ve 2'den küçük bir değer, başka birine bağımlı formülün hesaplanmasını imkansız kılar. Bu yüzden belirtilen değer 2'den küçükse, 2'ye sıfırlanacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalcStackSizeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Yığın hesaplaması gerektirecek örnek formülleri ayarlayın.
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // Özel yığın boyutuyla hesaplayın.
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


