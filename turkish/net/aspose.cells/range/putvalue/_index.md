---
title: "Range.PutValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Değeri aralığa koyar; uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrelerin sayı biçimi sıfırlanır"
type: docs
url: /tr/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Bir değeri aralığa koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | String | Giriş değeri |
| isConverted | Boolean | Doğru: uygun ise başka veri tipine dönüştürüldü. |
| setStyle | Boolean | Doğru: başka veri tipine dönüştürürken sayı formatını hücrenin stiline ayarla |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            
            Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


