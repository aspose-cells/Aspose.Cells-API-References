---
title: "LowCodeHtmlSaveOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeHtmlSaveOptions sınıfı. Düşük kod yöntemiyle HTML kaydetme seçenekleri"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/
---
## LowCodeHtmlSaveOptions class

Düşük kodlu bir şekilde HTML kaydetme seçenekleri.

```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | HTML kaydetme için genel seçenekler. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır ve ayarlar. Bu özelliği null veya boş dize dışındaki bir değerle ayarladığınızda, [`OutputStream`](../lowcodesaveoptions/outputstream/) yok sayılacaktır. ([`LowCodeSaveOptions`](../lowcodesaveoptions/) sınıfından devralınmıştır.) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null dışındaki bir değerle ayarladığınızda, [`OutputFile`](../lowcodesaveoptions/outputfile/) yok sayılacaktır. ([`LowCodeSaveOptions`](../lowcodesaveoptions/) sınıfından devralınmıştır.) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | Çalışma sayfasının formatını alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(29.99);

            // LowCodeHtmlSaveOptions oluştur ve yapılandır
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                HtmlOptions = new HtmlSaveOptions()
                {
                    ExportWorksheetCSSSeparately = false,
                    ExportImagesAsBase64 = true
                }
            };

            // Kaydetme seçenekleri parametresini kullanarak yapılandırılmış HTML seçenekleriyle çalışma kitabını kaydet
            workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);

            Console.WriteLine("HTML file saved successfully with low code options.");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


