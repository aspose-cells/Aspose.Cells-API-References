---
title: "Class GridSheetRender"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.Data.GridSheetRender sınıfı. Çalışma sayfasını BMP, PNG, JPEG, TIFF gibi çeşitli görüntülere render edebilen bir çalışma sayfası render'ını temsil eder. Bu sınıfın yapıcı, sayfa ayarı hücre stili değiştirildikten sonra kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

Bir çalışma sayfası render'ını temsil eder; bu render, çalışma sayfasını (BMP, PNG, JPEG, TIFF..) gibi çeşitli görüntülere dönüştürebilir. Bu sınıfın yapıcı yöntemi, sayfa ayarı ve hücre stilinde değişiklik yapıldıktan sonra kullanılmalıdır.

```csharp
public class GridSheetRender
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | SheetRender'in yapısı, parametre olarak çalışma sayfası ve ImageOrPrintOptions gerektirir |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | Geçerli çalışma sayfasının toplam sayfa sayısını alır. |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | Sayfanın hesaplanan ölçeğini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu al. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | Belirli bir sayfayı Bitmap nesnesine render eder. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | Belirli bir sayfayı akıma render eder. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | Belirli bir sayfayı bir dosyaya render eder. |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Belirli bir sayfayı Graphics'e render et |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Belirli bir sayfayı Graphics'e render et |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | Çalışma sayfasını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | Çalışma sayfasını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Çalışma sayfasını Yazıcıya render et |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | Çalışma sayfasını Yazıcıya render et |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | Tüm çalışma sayfasını Tiff Image olarak akışa render et. |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | Tüm çalışma sayfasını Tiff Image olarak bir dosyaya render et. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


