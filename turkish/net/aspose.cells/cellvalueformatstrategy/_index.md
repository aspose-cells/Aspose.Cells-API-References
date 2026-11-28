---
title: "CellValueFormatStrategy enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellValueFormatStrategy enum'ı. Hücre değerine stilin nasıl uygulanacağını belirtir"
type: docs
url: /tr/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

Hücrenin değeri için stilin nasıl uygulanacağını belirtir.

```csharp
public enum CellValueFormatStrategy
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Biçimlendirilmemiş. |
| CellStyle | `1` | Yalnızca hücrenin orijinal stiliyle biçimlendirilir. |
| DisplayStyle | `2` | Hücrenin görüntülenen stiliyle biçimlendirilir. |
| DisplayString | `3` | MS Excel'de gösterilen görüntülenen dizeyi alır. DisplayStyle'dan temel fark, bu seçeneğin ayrıca sütun genişliğinin etkisini de göz önünde bulundurmasıdır. Sütun genişliği biçimlendirilmiş dizeyi tamamen gösterecek kadar küçükse, MS Excel'in yaptığı gibi "#" gösterilebilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // Farklı CellValueFormatStrategy'leri uygulayarak etkilerini gösterin
            // None: Biçimlendirilmemiş
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle: Yalnızca hücrenin orijinal stiliyle biçimlendirilir
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle: Hücrenin görüntülenen stiliyle biçimlendirilir
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString: MS Excel'de gösterilen görüntülenen dizeyi alır
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // Çalışma kitabını bir dosyaya kaydedin
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


