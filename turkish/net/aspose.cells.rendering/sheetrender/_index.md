---
title: "Sınıf SheetRender"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.SheetRender sınıfı. Çalışma sayfasını BMP, PNG, JPEG, TIFF gibi çeşitli görüntülere render edebilen bir çalışma sayfası renderını temsil eder. Bu sınıfın yapıcı metodu, sayfa ayarı hücre stilinin değiştirilmesinden sonra kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Bir çalışma sayfası render'ını temsil eder; bu render, çalışma sayfasını (BMP, PNG, JPEG, TIFF..) gibi çeşitli görüntülere dönüştürebilir. Bu sınıfın yapıcı yöntemi, sayfa ayarı ve hücre stilinde değişiklik yapıldıktan sonra kullanılmalıdır.

```csharp
public class SheetRender
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | SheetRender'in yapısı, parametre olarak çalışma sayfası ve ImageOrPrintOptions gerektirir |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Geçerli çalışma sayfasının toplam sayfa sayısını alır. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Sayfanın hesaplanan ölçeğini alır. [`Zoom`](../../aspose.cells/pagesetup/zoom/) ayarlıysa ayarlanan ölçeği döndürür. Aksi takdirde, [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) ve [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/) değerlerine göre hesaplanan ölçeği döndürür. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | İstemci, bu işlevi kullanarak her sayfayı yazdırırken yazıcının sayfa ayarını kontrol edebilir. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Render için oluşturulan ve kullanılan kaynakları serbest bırakır. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu al. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Belirli bir sayfayı Bitmap nesnesine render eder. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Belirli bir sayfayı akıma render eder. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Belirli bir sayfayı bir dosyaya render eder. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Belirli bir sayfayı Graphics'e render et |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Belirli bir sayfayı Graphics'e render et |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Çalışma sayfasını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Çalışma sayfasını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Çalışma sayfasını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Çalışma sayfasını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Çalışma sayfasını Yazıcıya render et |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Tüm çalışma sayfasını Tiff Image olarak akışa render et. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Tüm çalışma sayfasını Tiff Image olarak bir dosyaya render et. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Sayfa ayarlarını yapılandır
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // SheetRender oluştur ve temel işlevselliği göster
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // İlk sayfayı görüntüye render et (demonstration)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


