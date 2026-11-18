---
title: "WorkbookRender Sınıfı"
linktitle: "WorkbookRender"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "WorkbookRender sınıfı. Go'da workbookrender'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/workbookrender/
---

## WorkbookRender class

Bir Çalışma Kitabı render'ını temsil eder. Bu sınıfın yapıcı yöntemi, sayfa ayarı ve hücre stili değiştirildikten sonra kullanılmalıdır.

```go

type WorkbookRender struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewWorkbookRender](./newworkbookrender/) | WorkbookRender'in yapısı |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetPageCount](./getpagecount/) | Çalışma kitabının toplam sayfa sayısını alır. |
| [GetPageSizeInch](./getpagesizeinch/) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu al. |
| [ToImage](./toimage/) | Tüm çalışma kitabını Tiff Görüntüsü olarak akışa render et. |
| [ToImage_String](./toimage_string/) | Tüm çalışma kitabını Tiff Görüntüsü olarak bir dosyaya render et. |
| [ToImage_Int_String](./toimage_int_string/) | Belirli bir sayfayı bir dosyaya render et. |
| [ToImage_Int](./toimage_int/) | Belirli bir sayfayı bir akışa render et. |
| [Dispose](./dispose/) | Render için oluşturulan ve kullanılan kaynakları serbest bırakır. |
