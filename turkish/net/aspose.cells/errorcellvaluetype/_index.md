---
title: "Enum ErrorCellValueType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ErrorCellValueType enum. Hata içeren bir hücre değerini temsil eder."
type: docs
url: /tr/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Bir hata içeren hücre değerini temsil eder.

```csharp
public enum ErrorCellValueType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Value | `1` | Bir hücrede #VALUE! hatası içeren değeri temsil eder. |
| Ref | `3` | Bir hücrede #REF! hatası içeren değeri temsil eder. |
| Name | `4` | Bir hücrede #NAME? hatası içeren değeri temsil eder. |
| NA | `6` | Bir hücrede #N/A hatası içeren değeri temsil eder. |
| Blocked | `10` | Bir hücrede #BLOCKED! hatası içeren değeri temsil eder. |
| Busy | `14` | Bir hücrede #BUSY! hatası içeren değeri temsil eder. |
| Calc | `13` | Bir hücrede #CALC! hatası içeren değeri temsil eder. |
| Connect | `9` | Bir hücrede #CONNECT! hatası içeren değeri temsil eder. |
| Field | `12` | Bir hücrede #FIELD! hatası içeren değeri temsil eder. |
| Spill | `8` | Bir hücrede #SPILL! hatası içeren değeri temsil eder. |
| Unknown | `11` | Bir hücrede #UNKNOWN! hatası içeren değeri temsil eder. |
| TimeOut | `19` | Bir hücrede #TIMEOUT! hatası içeren değeri temsil eder. |
| External | `18` | Bir hücrede #EXTERNAL! hatası içeren değeri temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir dökülme hatasına neden olacak bir formül ayarlayın.
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // Hatanın tetiklenmesi için formülleri hesaplayın.
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Beklenen dökülme hatası
            }
            
            // Hücrenin zengin değerini alın
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Hata tipini kontrol edin
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


