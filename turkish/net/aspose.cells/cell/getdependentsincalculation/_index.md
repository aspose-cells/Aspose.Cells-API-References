---
title: "Cell.GetDependentsInCalculation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri alır"
type: docs
url: /tr/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri al.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| recursive | Boolean | Bu, bu hücreye doğrudan referans vermeyen ancak bu hücrenin diğer yapraklarına referans veren bağımlılıkları döndürür mü |

### Dönüş Değeri

Tüm bağımlılıkları (Cell nesneleri) listelemek için Enumerator

### Açıklamalar

Bu yöntemi kullanmak için, çalışma kitabının [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) için true değerine ayarlandığından ve bu ayarla tamamen hesaplandığından emin olun. Bu hücreye formül referansı yoksa, null döndürülecektir.

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsInCalculationWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
            Console.WriteLine("B1's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
            
            en = cells["B2"].GetDependentsInCalculation(false);
            Console.WriteLine("B2's calculation dependents:");
            while(en.MoveNext())
            {
                Cell c = (Cell)en.Current;
                Console.WriteLine(c.Name);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


