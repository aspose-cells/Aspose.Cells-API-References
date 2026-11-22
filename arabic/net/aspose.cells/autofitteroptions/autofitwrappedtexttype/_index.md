---
title: "AutoFitterOptions.AutoFitWrappedTextType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AutoFitterOptions. تحصل وتضبط نوع النص الملتف تلقائيًا"
type: docs
url: /ar/net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

يحصل ويضبط نوع ضبط النص الملتف تلقائيًا.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### أمثلة

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
            
            // وصول ثابت إلى النمط باستخدام نمط GetStyle/SetStyle
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

### انظر أيضًا

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


