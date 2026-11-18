---
title: "FormulaSettings Sınıfı"
linktitle: "FormulaSettings"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FormulaSettings sınıfı. Go'da formulasettings'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/formulasettings/
---

## FormulaSettings class

Formüllerin ve hesaplamanın ayarları.

```go

type FormulaSettings struct  {
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
| [GetCalculateOnOpen](./getcalculateonopen/) | Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini belirtir. |
| [SetCalculateOnOpen](./setcalculateonopen/) | Uygulamanın çalışma kitabı açıldığında tam bir hesaplama yapması gerekip gerekmediğini belirtir. |
| [GetCalculateOnSave](./getcalculateonsave/) | Manuel hesaplama modunda belgeyi kaydetmeden önce çalışma kitabını yeniden hesaplayıp hesaplamayacağını belirtir. |
| [SetCalculateOnSave](./setcalculateonsave/) | Manuel hesaplama modunda belgeyi kaydetmeden önce çalışma kitabını yeniden hesaplayıp hesaplamayacağını belirtir. |
| [GetForceFullCalculation](./getforcefullcalculation/) | Bir hesaplama tetiklendiğinde her seferinde tüm formülleri hesaplayıp hesaplamadığını belirtir. |
| [SetForceFullCalculation](./setforcefullcalculation/) | Bir hesaplama tetiklendiğinde her seferinde tüm formülleri hesaplayıp hesaplamadığını belirtir. |
| [GetCalculationMode](./getcalculationmode/) | MS Excel'de çalışma kitabı hesaplaması için modu alır veya ayarlar. |
| [SetCalculationMode](./setcalculationmode/) | MS Excel'de çalışma kitabı hesaplaması için modu alır veya ayarlar. |
| [GetCalculationId](./getcalculationid/) | Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir. |
| [SetCalculationId](./setcalculationid/) | Çalışma kitabındaki değerleri hesaplamak için kullanılan hesaplama motorunun sürümünü belirtir. |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | Döngüsel referansları çözmek için yinelemeli hesaplamayı etkinleştirip etkinleştirilmeyeceğini gösterir. |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | Döngüsel referansları çözmek için yinelemeli hesaplamayı etkinleştirip etkinleştirilmeyeceğini gösterir. |
| [GetMaxIteration](./getmaxiteration/) | Döngüsel bir referansı çözmek için maksimum yineleme sayısı. |
| [SetMaxIteration](./setmaxiteration/) | Döngüsel bir referansı çözmek için maksimum yineleme sayısı. |
| [GetMaxChange](./getmaxchange/) | Döngüsel bir referansı çözmek için maksimum değişim. |
| [SetMaxChange](./setmaxchange/) | Döngüsel bir referansı çözmek için maksimum değişim. |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | Formüller hesaplanırken hesaplanan sonucun hassasiyetinin görüntülendikleri gibi ayarlanıp ayarlanmayacağını gösterir. |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | Formüller hesaplanırken hesaplanan sonucun hassasiyetinin görüntülendikleri gibi ayarlanıp ayarlanmayacağını gösterir. |
| [GetEnableCalculationChain](./getenablecalculationchain/) | Formüller için hesaplama zincirini etkinleştirip etkinleştirilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [SetEnableCalculationChain](./setenablecalculationchain/) | Formüller için hesaplama zincirini etkinleştirip etkinleştirilmeyeceğini gösterir. Varsayılan değer false'tur. |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur. |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur. |
