---
title: "Cell.GetPrecedentsInCalculation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücrenin formülü hesaplanırken mevcut çalışma kitabındaki hücrelere yapılan tüm önceki referansları alır"
type: docs
url: /tr/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Bu hücrenin formülü hesaplanırken kullandığı tüm öncülleri (geçerli çalışma kitabındaki hücre referansları) al.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Dönüş Değeri

Tüm referansları (ReferredArea) listelemek için Enumerator

### Açıklamalar

Bu yöntem yalnızca çalışma kitabı için [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) özelliği true olduğunda ve çalışma kitabı tamamen hesaplandığında çalışabilir. Eğer bu hücre bir formül değilse veya başka hücrelere referans vermiyorsa, null döndürülür.

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsInCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["B1"].PutValue(10);
            cells["B2"].PutValue(20);
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
            Console.WriteLine("A2's calculation precedents:");
            while(en.MoveNext())
            {
                ReferredArea r = (ReferredArea)en.Current;
                Console.WriteLine(r);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


