---
title: "DrawObject Sınıfı"
linktitle: "DrawObject"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DrawObject sınıfı. Go'da drawobject'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/drawobject/
---

## DrawObject class

Renderleme sırasında DrawObject başlatılacak ve döndürülecek.

```go

type DrawObject struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetCell](./getcell/) | Render ederken Cell nesnesini gösterir. Hücrenin tüm özelliklerine erişilebilir. |
| [GetShape](./getshape/) | Render ederken Shape nesnesini gösterir. Şeklin tüm özelliklerine erişilebilir. |
| [GetImageBytes](./getimagebytes/) | Render edilen Chart ve Shape'in görüntü baytlarını gösterir. |
| [GetType](./gettype/) | DrawObject'in tipini gösterir. |
| [GetCurrentPage](./getcurrentpage/) | DrawObject'in sayfa indeksini gösterir. Sayfa indeksi sıfırdan başlar. Bir Sheet render ederken birden fazla sayfa içerir. |
| [GetTotalPages](./gettotalpages/) | Mevcut render işleminin toplam sayfa sayısını gösterir. |
| [GetSheetIndex](./getsheetindex/) | DrawObject'in mevcut sheet indeksini gösterir. |
