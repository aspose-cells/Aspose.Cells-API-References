---
title: "Sınıf WorkbookRender"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.WorkbookRender sınıfı. Bir Çalışma Kitabı renderını temsil eder. Bu sınıfın yapıcı yöntemi, sayfa ayarı hücre stilinin değiştirilmesinden sonra kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Bir Çalışma Kitabı render'ını temsil eder. Bu sınıfın yapıcı yöntemi, sayfa ayarı ve hücre stilinde değişiklik yapıldıktan sonra kullanılmalıdır.

```csharp
public class WorkbookRender
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | WorkbookRender'in yapısı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Çalışma kitabının toplam sayfa sayısını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | İstemci, bu işlevi kullanarak her sayfayı yazdırırken yazıcının sayfa ayarını kontrol edebilir. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Render için oluşturulan ve kullanılan kaynakları serbest bırakır. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu al. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Belirli bir sayfayı Bitmap nesnesine render eder. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Tüm çalışma kitabını Tiff Görüntüsü olarak akıma render eder. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Tüm çalışma kitabını Tiff Görüntüsü olarak bir dosyaya render eder. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Belirli bir sayfayı akıma render eder. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Belirli bir sayfayı bir dosyaya render eder. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Çalışma kitabını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Çalışma kitabını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Çalışma kitabını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Çalışma kitabını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Çalışma kitabını Yazıcıya render et |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekle ve sayfa boyutunu ayarla
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Çalışma kitabı oluştur, render et ve sayfa boyutunu al
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // Sonuçları çıktı olarak ver.
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


