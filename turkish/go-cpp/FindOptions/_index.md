---
title: "FindOptions Sınıfı"
linktitle: "FindOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FindOptions sınıfı. Go dilinde findoptions nesnesini temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/findoptions/
---

## FindOptions class

Bulma seçeneklerini temsil eder.

```go

type FindOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewFindOptions](./newfindoptions/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetCaseSensitive](./getcasesensitive/) | Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir. |
| [SetCaseSensitive](./setcasesensitive/) | Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir. |
| [GetLookAtType](./getlookattype/) | Bakılan tür. |
| [SetLookAtType](./setlookattype/) | Bakılan tür. |
| [GetRange](./getrange/) | Aranan aralığı alır ve ayarlar. |
| [SetRange](./setrange/) | Aranan aralığı ayarlar. |
| [IsRangeSet](./israngeset/) | Aranan aralığın ayarlanıp ayarlanmadığını gösterir. |
| [GetSearchBackward](./getsearchbackward/) | Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir. |
| [SetSearchBackward](./setsearchbackward/) | Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir. |
| [GetSearchOrderByRows](./getsearchorderbyrows/) | Arama sırasının satır mı yoksa sütun mu olduğunu gösterir. |
| [SetSearchOrderByRows](./setsearchorderbyrows/) | Arama sırasının satır mı yoksa sütun mu olduğunu gösterir. |
| [GetLookInType](./getlookintype/) | İçinde bakılan tür. |
| [SetLookInType](./setlookintype/) | İçinde bakılan tür. |
| [GetRegexKey](./getregexkey/) | Aranan anahtarın regex olup olmadığını gösterir.Eğer doğruysa aranan anahtar regex olarak alınır ve ayrıştırılır.Aksi takdirde anahtar MS Excel kurallarına göre ayrıştırılır. |
| [SetRegexKey](./setregexkey/) | Aranan anahtarın regex olup olmadığını gösterir.Eğer doğruysa aranan anahtar regex olarak alınır ve ayrıştırılır.Aksi takdirde anahtar MS Excel kurallarına göre ayrıştırılır. |
| [GetValueTypeSensitive](./getvaluetypesensitive/) | Aranan hücre değer tipinin aranan anahtar ile aynı olması gerekip gerekmediğini gösterir. |
| [SetValueTypeSensitive](./setvaluetypesensitive/) | Aranan hücre değer tipinin aranan anahtar ile aynı olması gerekip gerekmediğini gösterir. |
| [GetStyle](./getstyle/) | Aranacak format. |
| [SetStyle](./setstyle/) | Aranacak format. |
| [GetConvertNumericData](./getconvertnumericdata/) | Aranan dize değerinin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [SetConvertNumericData](./setconvertnumericdata/) | Aranan dize değerinin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değeri alır veya ayarlar. |
