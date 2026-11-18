---
title: "SheetRender Sınıf"
linktitle: "SheetRender"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SheetRender sınıfı. Go'da sheetrender'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/sheetrender/
---

## SheetRender class

Çalışma sayfasını çeşitli görüntülere (BMP, PNG, JPEG, TIFF..) renderleyebilen bir çalışma sayfası render'ını temsil eder. Bu sınıfın yapıcı yöntemi, sayfa ayarı ve hücre stili değiştirildikten sonra kullanılmalıdır.

```go

type SheetRender struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewSheetRender](./newsheetrender/) | SheetRender'ın yapısı, parametre olarak çalışma sayfası ve ImageOrPrintOptions gerektirir. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetPageCount](./getpagecount/) | Mevcut çalışma sayfasının toplam sayfa sayısını alır. |
| [GetPageScale](./getpagescale/) | Sayfanın hesaplanan sayfa ölçeğini alır. PageSetup.Zoom ayarlanmışsa belirlenen ölçeği döndürür. Aksi takdirde, PageSetup.FitToPagesWide ve PageSetup.FitToPagesTall değerlerine göre hesaplanan ölçeği döndürür. |
| [GetPageSizeInch](./getpagesizeinch/) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu al. |
| [ToImage_Int_String](./toimage_int_string/) | Belirli bir sayfayı bir dosyaya render et. |
| [ToImage_Int](./toimage_int/) | Belirli bir sayfayı bir akışa render et. |
| [ToTiff](./totiff/) | Tüm çalışma sayfasını Tiff Görüntüsü olarak akıma render eder. |
| [ToTiff_String](./totiff_string/) | Tüm çalışma sayfasını Tiff Görüntüsü olarak bir dosyaya render eder. |
| [Dispose](./dispose/) | Render için oluşturulan ve kullanılan kaynakları serbest bırakır. |
