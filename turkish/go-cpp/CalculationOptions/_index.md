---
title: "CalculationOptions Sınıfı"
linktitle: "CalculationOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CalculationOptions sınıfı. Go dilinde calculationoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/calculationoptions/
---

## CalculationOptions class

Hesaplama seçeneklerini temsil eder.

```go

type CalculationOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewCalculationOptions](./newcalculationoptions/) | Varsayılan yapıcı. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetIgnoreError](./getignoreerror/) | Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmeyeceğini gösterir.Hata, desteklenmeyen işlev, dış bağlantılar vb. olabilir.Varsayılan değer true'dur. |
| [SetIgnoreError](./setignoreerror/) | Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmeyeceğini gösterir.Hata, desteklenmeyen işlev, dış bağlantılar vb. olabilir.Varsayılan değer true'dur. |
| [GetRecursive](./getrecursive/) | Bir hücre hesaplanırken ve diğer hücrelere bağlı olduğunda bağımlı hücrelerin yinelemeli olarak hesaplanıp hesaplanmayacağını gösterir.Varsayılan değer true'dur. |
| [SetRecursive](./setrecursive/) | Bir hücre hesaplanırken ve diğer hücrelere bağlı olduğunda bağımlı hücrelerin yinelemeli olarak hesaplanıp hesaplanmayacağını gösterir.Varsayılan değer true'dur. |
| [GetUserSpecifiedRefreshDynamicArrayFormula](./getuserspecifiedrefreshdynamicarrayformula/) | Kullanıcının, belirtilen formüller hesaplanmadan önce dinamik dizi formüllerinin yenilenme davranışını açıkça belirleyip belirlemediğini gösterir. |
| [GetRefreshDynamicArrayFormula](./getrefreshdynamicarrayformula/) | Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir. |
| [SetRefreshDynamicArrayFormula](./setrefreshdynamicarrayformula/) | Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir. |
| [GetCustomEngine](./getcustomengine/) | Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru. |
| [SetCustomEngine](./setcustomengine/) | Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru. |
| [GetCalcStackSize](./getcalcstacksize/) | Hücreleri yinelemeli olarak hesaplamak için yığın boyutu. Varsayılan değer 200. |
| [SetCalcStackSize](./setcalcstacksize/) | Hücreleri yinelemeli olarak hesaplamak için yığın boyutu. Varsayılan değer 200. |
| [GetPrecisionStrategy](./getprecisionstrategy/) | Hesaplama hassasiyetinin işlenmesi için stratejiyi belirtir. |
| [SetPrecisionStrategy](./setprecisionstrategy/) | Hesaplama hassasiyetinin işlenmesi için stratejiyi belirtir. |
| [GetLinkedDataSources](./getlinkeddatasources/) | Formüllerde kullanılan dış bağlantılar için veri kaynaklarını belirtir. |
| [SetLinkedDataSources](./setlinkeddatasources/) | Formüllerde kullanılan dış bağlantılar için veri kaynaklarını belirtir. |
| [GetCharacterEncoding](./getcharacterencoding/) | Formüller hesaplanırken karakterlerin kodlanması/çözülmesi için kullanılan kodlamayı belirtir. CHAR, CODE gibi işlevler için hesaplanan sonuç, bölge ayarları ve ortamın varsayılan karakter kümesine bağlıdır. Bu özellik sayesinde kullanıcı, bu işlevler için beklenen sonucu elde etmek amacıyla kullanılacak uygun kodlamayı belirtebilir. |
| [SetCharacterEncoding](./setcharacterencoding/) | Formüller hesaplanırken karakterlerin kodlanması/çözülmesi için kullanılan kodlamayı belirtir. CHAR, CODE gibi işlevler için hesaplanan sonuç, bölge ayarları ve ortamın varsayılan karakter kümesine bağlıdır. Bu özellik sayesinde kullanıcı, bu işlevler için beklenen sonucu elde etmek amacıyla kullanılacak uygun kodlamayı belirtebilir. |
