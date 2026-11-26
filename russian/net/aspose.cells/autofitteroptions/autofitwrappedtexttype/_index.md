---
title: "AutoFitterOptions.AutoFitWrappedTextType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Получает и задает тип автоподгонки перенесённого текста"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Получает и задает тип автоматической подгонки перенесённого текста.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Примеры

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
            
            // Фиксированный доступ к стилю с использованием шаблона GetStyle/SetStyle
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

### См. также

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


