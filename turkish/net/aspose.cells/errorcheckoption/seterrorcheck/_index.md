---
title: "ErrorCheckOption.SetErrorCheck"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ErrorCheckOption yöntemi. Belirtilen hata türünün kontrol edilip edilmeyeceğini ayarlar"
type: docs
url: /tr/net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

Verilen hata tipinin kontrol edilip edilmeyeceğini ayarlar.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | hata türü kontrol edilebilir. |
| isCheck | Boolean | verilen hata türünün kontrol edilmesi gerekiyorsa true (kontrol başarısız olursa hücrede yeşil üçgen gösterilir). |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Sample text for error checking");
            
            // Hata kontrol seçeneklerini yapılandırın
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            
            // SetErrorCheck'i farklı ErrorCheckType değerleriyle gösterin
            errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            
            // Tüm çalışma sayfasına uygula
            errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
            
            workbook.Save("ErrorCheckExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


