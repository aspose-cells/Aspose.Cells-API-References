---
title: "HtmlSaveOptions.CssStyles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Biçimlendirici için ek css stillerini alır veya ayarlar. Yalnızca SaveAsSingleFile True olduğunda çalışır.  CssStylesbody  padding 5px"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/cssstyles/
---
## HtmlSaveOptions.CssStyles property

Biçimlendirici için ek css stillerini alır veya ayarlar. Yalnızca [`SaveAsSingleFile`](../saveassinglefile/) True olduğunda çalışır.  CssStyles="body { padding: 5px }";

```csharp
public string CssStyles { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCssStylesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Özel CSS stillerini ayarlayın
            saveOptions.CssStyles = @"
                body { 
                    font-family: Arial;
                    background-color: #f0f0f0;
                }
                table {
                    border-collapse: collapse;
                    width: 100%;
                }
                td {
                    border: 1px solid #ddd;
                    padding: 8px;
                }";

            // Çalışma kitabını özel CSS stilleriyle kaydedin
            workbook.Save("HtmlWithCustomStyles.html", saveOptions);

            Console.WriteLine("HTML file with custom CSS styles created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


