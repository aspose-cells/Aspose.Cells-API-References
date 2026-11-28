---
title: "ErrorCheckOption.IsErrorCheck"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ErrorCheckOption yöntemi. Belirtilen hata türünün kontrol edilip edilmeyeceğini denetler"
type: docs
url: /tr/net/aspose.cells/errorcheckoption/iserrorcheck/
---
## ErrorCheckOption.IsErrorCheck method

Verilen hata tipinin kontrol edilip edilmeyeceğini denetler.

```csharp
public bool IsErrorCheck(ErrorCheckType errorCheckType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | hata türü kontrol edilebilir |

### Dönüş Değeri

verilen hata türü kontrol edilecekse true döndürür (kontrol başarısız olursa hücrede yeşil üçgen gösterilir).

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodIsErrorCheckWithErrorCheckTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            int index = options.Add();
            ErrorCheckOption option = options[index];

            // Hata kontrol ayarlarını yapılandırın
            option.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            option.SetErrorCheck(ErrorCheckType.EvaluationError, true);
            option.SetErrorCheck(ErrorCheckType.InconsistRange, false);

            // Bu ayarları uygulamak için aralık ekle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 10;
            area.StartColumn = 0;
            area.EndColumn = 5;
            option.AddRange(area);

            // Ayarları doğrula ve göster
            Console.WriteLine("NumberStoredAsText check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.NumberStoredAsText));
            Console.WriteLine("EvaluationError check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.EvaluationError));
            Console.WriteLine("InconsistRange check enabled: " + 
                option.IsErrorCheck(ErrorCheckType.InconsistRange));
        }
    }
}
```

### Ayrıca Bakınız

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


