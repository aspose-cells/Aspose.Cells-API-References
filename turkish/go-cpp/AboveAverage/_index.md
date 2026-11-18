---
title: "AboveAverage Sınıfı"
linktitle: "AboveAverage"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "AboveAverage sınıfı. Go'da aboveaverage nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/aboveaverage/
---

## AboveAverage class

AboveAverage koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki veya altındaki hücreleri vurgular.

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsAboveAverage](./isaboveaverage/) | Kuralın \"above average\" (ortalamanın üzeri) kuralı olup olmadığını gösteren bayrağı alır veya ayarlar. 'true' değeri 'above average' olduğunu gösterir. Varsayılan değer true'tur. |
| [SetIsAboveAverage](./setisaboveaverage/) | Kuralın \"above average\" (ortalamanın üzeri) kuralı olup olmadığını gösteren bayrağı alır veya ayarlar. 'true' değeri 'above average' olduğunu gösterir. Varsayılan değer true'tur. |
| [IsEqualAverage](./isequalaverage/) | Ortalamanın kendisini içerecek şekilde 'aboveAverage' ve 'belowAverage' kriterlerinin kapsayıcı olup olmadığını gösteren bayrağı alır veya ayarlar, ya da bu değerden hariç tutar. 'true' değeri ortalama değerin kriterde dahil edilmesini gösterir. Varsayılan değer false'tur. |
| [SetIsEqualAverage](./setisequalaverage/) | Ortalamanın kendisini içerecek şekilde 'aboveAverage' ve 'belowAverage' kriterlerinin kapsayıcı olup olmadığını gösteren bayrağı alır veya ayarlar, ya da bu değerden hariç tutar. 'true' değeri ortalama değerin kriterde dahil edilmesini gösterir. Varsayılan değer false'tur. |
| [GetStdDev](./getstddev/) | Ortalamanın üzerindeki veya altındaki standart sapma sayısını koşullu biçimlendirme kuralına dahil etmek için alır veya ayarlar. Giriş değeri 0 ile 3 arasında olmalıdır (0 ve 3 dahil). Bu değeri 0 olarak ayarlamak, stdDev'in ayarlanmadığı anlamına gelir. Varsayılan değer 0'tır. |
| [SetStdDev](./setstddev/) | Ortalamanın üzerindeki veya altındaki standart sapma sayısını koşullu biçimlendirme kuralına dahil etmek için alır veya ayarlar. Giriş değeri 0 ile 3 arasında olmalıdır (0 ve 3 dahil). Bu değeri 0 olarak ayarlamak, stdDev'in ayarlanmadığı anlamına gelir. Varsayılan değer 0'tır. |
