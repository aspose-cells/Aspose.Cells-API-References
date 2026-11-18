---
title: "PdfBookmarkEntry Sınıfı"
linktitle: "PdfBookmarkEntry"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PdfBookmarkEntry sınıf. Go'da pdfbookmarkentry'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry, pdf yer işaretinde bir giriştir. Eğer mevcut örneğin Text özelliği null veya "" ise, mevcut örnek gizlenecek ve alt öğeler aynı seviyeye eklenecektir.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetText](./gettext/) | Yer işaretinin başlığı. |
| [SetText](./settext/) | Yer işaretinin başlığı. |
| [GetDestination](./getdestination/) | Yer işareti bağlantısının yönlendirildiği hücre. |
| [SetDestination](./setdestination/) | Yer işareti bağlantısının yönlendirildiği hücre. |
| [GetDestinationName](./getdestinationname/) | Hedefin adını alır veya ayarlar. |
| [SetDestinationName](./setdestinationname/) | Hedefin adını alır veya ayarlar. |
| [IsOpen](./isopen/) | Bu özellik true olduğunda, yer işareti girişi genişleyecek, aksi takdirde daralacaktır. |
| [SetIsOpen](./setisopen/) | Bu özellik true olduğunda, yer işareti girişi genişleyecek, aksi takdirde daralacaktır. |
| [IsCollapse](./iscollapse/) | Bu özellik true olduğunda, yer işareti girişi daralacak, aksi takdirde genişleyecektir. |
| [SetIsCollapse](./setiscollapse/) | Bu özellik true olduğunda, yer işareti girişi daralacak, aksi takdirde genişleyecektir. |
