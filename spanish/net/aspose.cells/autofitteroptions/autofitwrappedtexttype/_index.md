---
title: "AutoFitterOptions.AutoFitWrappedTextType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Obtiene y establece el tipo de ajuste automático de texto envuelto"
type: docs
url: /es/net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Obtiene y establece el tipo de ajuste automático del texto envuelto.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Ejemplos

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
            
            // Acceso a estilo fijo usando el patrón GetStyle/SetStyle
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

### Ver también

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


