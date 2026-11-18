---
title: "Name Sınıfı"
linktitle: "Name"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Name sınıfı. Go'da name'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/name/
---

## Name class

Hücre aralığı için tanımlanmış bir adı temsil eder.

```go

type Name struct  {
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
| [GetComment](./getcomment/) | Name'in yorumunu alır ve ayarlar. Yalnızca Excel 2007 veya daha yeni sürümler için geçerlidir. |
| [SetComment](./setcomment/) | Name'in yorumunu alır ve ayarlar. Yalnızca Excel 2007 veya daha yeni sürümler için geçerlidir. |
| [GetText](./gettext/) | Nesnenin ad metnini alır. |
| [SetText](./settext/) | Nesnenin ad metnini alır. |
| [GetFullText](./getfulltext/) | Nesnenin kapsam ayarıyla adının tam metnini alır. |
| [GetRefersTo](./getrefersto/) | İsmin başvurmak üzere tanımlandığı formülü döndürür veya ayarlar, eşittir işaretiyle başlar. |
| [SetRefersTo_String](./setrefersto_string/) | İsmin başvurmak üzere tanımlandığı formülü döndürür veya ayarlar, eşittir işaretiyle başlar. |
| [GetR1C1RefersTo](./getr1c1refersto/) | İsmin bir R1C1 referansını alır veya ayarlar. |
| [SetR1C1RefersTo](./setr1c1refersto/) | İsmin bir R1C1 referansını alır veya ayarlar. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Bu ismin referansını al. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Belirtilen hücreye göre bu ismin referansını al. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Bu ismin referansını ayarla. |
| [IsReferred](./isreferred/) | Bu ismin diğer formüller tarafından başvurulup başvurulmadığını gösterir. |
| [IsVisible](./isvisible/) | İsmin görünür olup olmadığını gösterir. |
| [SetIsVisible](./setisvisible/) | İsmin görünür olup olmadığını gösterir. |
| [GetSheetIndex](./getsheetindex/) | Bu ismin Çalışma Kitabı'na mı yoksa Çalışma Sayfası'na mı ait olduğunu gösterir.0 = Genel isim, aksi takdirde sayfaya indeks (tek tabanlı). |
| [SetSheetIndex](./setsheetindex/) | Bu ismin Çalışma Kitabı'na mı yoksa Çalışma Sayfası'na mı ait olduğunu gösterir.0 = Genel isim, aksi takdirde sayfaya indeks (tek tabanlı). |
| [ToString](./tostring/) | Geçerli Range nesnesini temsil eden bir dize döndürür. |
| [GetRanges](./getranges/) | Bu isim tarafından başvurulan tüm aralıkları alır. |
| [GetRanges_Bool](./getranges_bool/) | Bu isim tarafından başvurulan tüm aralıkları alır. |
| [GetReferredAreas](./getreferredareas/) | Bu isim tarafından başvurulan tüm referansları alır. |
| [GetRange](./getrange/) | Bu isim bir aralığa işaret ediyorsa aralığı alır. |
| [GetRange_Bool](./getrange_bool/) | Bu isim bir aralığa işaret ediyorsa aralığı alır |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | Bu isim bir aralığa işaret ediyorsa aralığı alır. Bu ismin referansı mutlak değilse, aralık farklı hücreler için farklı olabilir. |
