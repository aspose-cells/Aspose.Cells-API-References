---
title: "Sınıf ErrorCheckOption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ErrorCheckOption sınıfı. Belirli aralıklara uygulanan hata kontrol ayarı"
type: docs
url: /tr/net/aspose.cells/errorcheckoption/
---
## ErrorCheckOption class

Belirli aralıklara uygulanan hata kontrol ayarı.

```csharp
public class ErrorCheckOption
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddRange](../../aspose.cells/errorcheckoption/addrange/)(CellArea) | Bu ayar tarafından etkilenen bir aralık ekler. |
| [GetCountOfRange](../../aspose.cells/errorcheckoption/getcountofrange/)() | Bu ayar tarafından etkilenen aralıkların sayısını alır. |
| [GetRange](../../aspose.cells/errorcheckoption/getrange/)(int) | Verilen indeksle bu ayarın etkilediği aralığı alır. |
| [IsErrorCheck](../../aspose.cells/errorcheckoption/iserrorcheck/)(ErrorCheckType) | Verilen hata tipinin kontrol edilip edilmeyeceğini denetler. |
| [RemoveRange](../../aspose.cells/errorcheckoption/removerange/)(int) | Verilen indeksle bir aralığı kaldırır. |
| [SetErrorCheck](../../aspose.cells/errorcheckoption/seterrorcheck/)(ErrorCheckType, bool) | Verilen hata tipinin kontrol edilip edilmeyeceğini ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionDemo
    {
        public static void ErrorCheckOptionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasından ErrorCheckOptionCollection'ı alın
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Koleksiyona yeni bir ErrorCheckOption ekleyin
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Hata kontrol seçeneklerini ayarlayın
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Bir hücre alanı tanımlayın ve bunu ErrorCheckOption'a ekleyin
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Çalışma kitabını kaydedin
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


