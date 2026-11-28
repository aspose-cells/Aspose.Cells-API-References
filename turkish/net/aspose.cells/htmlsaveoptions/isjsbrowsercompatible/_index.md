---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. JavaScript'in JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'tur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

JavaScript'in JavaScript desteklemeyen tarayıcılarla uyumlu olup olmadığını gösterir. Varsayılan değer true'tur.

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // IsJsBrowserCompatible true olarak ayarlanmış HTML kaydetme seçeneklerini yapılandır
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // JavaScript uyumluluğu ile çalışma kitabını kaydet
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


