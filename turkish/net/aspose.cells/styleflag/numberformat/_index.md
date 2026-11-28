---
title: "StyleFlag.NumberFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Sayı biçimi ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Sayı biçimi ayarı uygulanacak.

```csharp
public bool NumberFormat { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hücre değerini ayarla
            sheet.Cells[0, 0].Value = 1234.56;
            
            // Özel sayı biçimi stili oluştur
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // Yalnızca sayı biçimini StyleFlag kullanarak uygula
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // Stili hücre aralığına uygula (Range tipini tam nitelendir)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // Kaydet ve doğrula
            workbook.Save("output_number_format.ods");
            
            // Doğrulamak için yeniden yükle
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


