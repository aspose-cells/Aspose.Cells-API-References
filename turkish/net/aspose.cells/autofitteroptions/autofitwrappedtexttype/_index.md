---
title: "AutoFitterOptions.AutoFitWrappedTextType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Sarılmış metnin otomatik sığdırma türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Satır sonu ile sarılmış metnin otomatik ayarlanma türünü alır ve ayarlar.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Örnekler

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitWrappedTextTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Cell cell = worksheet.Cells["A1"];
            cell.Value = "This is a sample text string that demonstrates auto-fitting wrapped text using Paragraph mode";
            
            // GetStyle/SetStyle desenini kullanarak sabit stil erişimi
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            };

            worksheet.AutoFitColumns(options);
            workbook.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Ayrıca Bakınız

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


