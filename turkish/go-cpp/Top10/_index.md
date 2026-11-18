---
title: "Top10 Sınıfı"
linktitle: "Top10"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Top10 sınıfı. Go'da top10'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/top10/
---

## Top10 class

Top10 koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, belirtilen şekilde, değerleri en üst N veya en alt N aralığına düşen hücreleri vurgular.

```go

type Top10 struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewTop10](./newtop10/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsPercent](./ispercent/) | Bir "top/bottom n" kuralının "top/bottom n yüzde" kuralı olup olmadığını alır veya ayarlar. Varsayılan değer false'tur. |
| [SetIsPercent](./setispercent/) | Bir "top/bottom n" kuralının "top/bottom n yüzde" kuralı olup olmadığını alır veya ayarlar. Varsayılan değer false'tur. |
| [IsBottom](./isbottom/) | Bir "top/bottom n" kuralının "bottom n" kuralı olup olmadığını alır veya ayarlar. Varsayılan değer false'tur. |
| [SetIsBottom](./setisbottom/) | Bir "top/bottom n" kuralının "bottom n" kuralı olup olmadığını alır veya ayarlar. Varsayılan değer false'tur. |
| [GetRank](./getrank/) | Bir "top/bottom n" koşullu biçimlendirme kuralındaki "n" değerini alır veya ayarlar. IsPercent true ise değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10'dur. |
| [SetRank](./setrank/) | Bir "top/bottom n" koşullu biçimlendirme kuralındaki "n" değerini alır veya ayarlar. IsPercent true ise değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10'dur. |
