---
title: "ErrorCheckType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ErrorCheckType enum'ı. Tüm hata kontrol türlerini temsil eder"
type: docs
url: /tr/net/aspose.cells/errorchecktype/
---
## ErrorCheckType enumeration

Tüm hata kontrol türlerini temsil eder.

```csharp
public enum ErrorCheckType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| EvaluationError | `1` | Hücreler hata üreten formüller içerdiğinde hataları yoksay. |
| Calc | `1` |  |
| EmptyCellRef | `2` | Formüller boş hücrelere başvurduğunda hataları yoksay. |
| NumberStoredAsText | `4` | Sayılar metin olarak biçimlendirildiğinde veya başında tek tırnak işareti olduğunda hataları yoksay. |
| TextNumber | `4` | Sayılar metin olarak biçimlendirildiğinde veya başında tek tırnak işareti olduğunda hataları yoksay. |
| InconsistRange | `8` | Formüller bir bölgede belirli hücreleri atladığında hataları yoksay. |
| InconsistFormula | `16` | Çalışma sayfanızdaki bir bölgedeki formül aynı bölgedeki diğer formüllerden farklı olduğunda hataları yoksay. |
| TwoDigitTextYear | `32` | Formüller, yılları 2 basamak olarak gösteren metin biçimli hücreler içerdiğinde hataları yoksay. |
| TextDate | `32` | Formüller, yılları 2 basamak olarak gösteren metin biçimli hücreler içerdiğinde hataları yoksay. |
| UnlockedFormula | `64` | Kilitlenmemiş hücreler formül içerdiğinde hataları yoksay. |
| UnproctedFormula | `64` | Kilitlenmemiş hücreler formül içerdiğinde hataları yoksay. |
| TableDataValidation | `128` | Bir Tablodaki hücrenin değeri belirtilen Veri Doğrulama kurallarına uymadığında hataları yoksay. |
| Validation | `128` | Bir Tablodaki hücrenin değeri belirtilen Veri Doğrulama kurallarına uymadığında hataları yoksay. |
| CalculatedColumn | `129` | Hücreler, hesaplanmış sütun formülünden farklı bir değer içerdiğinde hataları yoksay. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckTypeDemo
    {
        public static void ErrorCheckTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ErrorCheckOptionCollection öğesine erişin
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Yeni bir ErrorCheckOption ekleyin
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];

            // Çeşitli hata kontrol türlerini false olarak ayarlayın
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.Validation, false);

            // Hata kontrol seçeneği için bir hücre alanı tanımlayın
            CellArea cellArea = CellArea.CreateCellArea("A1", "B10");
            errorCheckOption.AddRange(cellArea);

            // Çalışma kitabını kaydedin
            workbook.Save("ErrorCheckTypeExample.xlsx");
            workbook.Save("ErrorCheckTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


