---
title: "FormatCondition Class"
linktitle: "FormatCondition"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FormatCondition class. Go'da formatcondition'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/formatcondition/
---

## FormatCondition class

Koşullu biçimlendirme koşulunu temsil eder.

```go

type FormatCondition struct  {
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
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır. |
| [SetFormulas](./setformulas/) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar. |
| [GetFormula1](./getformula1/) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [SetFormula1_String](./setformula1_string/) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [GetFormula1_Int_Int](./getformula1_int_int/) | Hücrenin koşullu biçimlendirmesinin formülünü alır. |
| [GetFormula2](./getformula2/) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [SetFormula2_String](./setformula2_string/) | Koşullu biçimlendirme ile ilişkili değeri veya ifadeyi alır ve ayarlar. |
| [GetFormula2_Int_Int](./getformula2_int_int/) | Hücrenin koşullu biçimlendirmesinin formülünü alır. |
| [GetOperator](./getoperator/) | Koşullu biçim operatör tipini alır ve ayarlar. |
| [SetOperator](./setoperator/) | Koşullu biçim operatör tipini alır ve ayarlar. |
| [GetStopIfTrue](./getstopiftrue/) | Doğru, bu kural doğru değerlendirildiğinde daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz. Yalnızca Excel 2007 için geçerlidir; |
| [SetStopIfTrue](./setstopiftrue/) | Doğru, bu kural doğru değerlendirildiğinde daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz. Yalnızca Excel 2007 için geçerlidir; |
| [GetPriority](./getpriority/) | Bu koşullu biçimlendirme kuralının önceliği. Bu değer, whichformatın değerlendirilip işleneceğini belirlemek için kullanılır. Daha düşük sayısal değerler, thanhigher sayısal değerlere göre daha yüksek önceliğe sahiptir, burada '1' en yüksek önceliği temsil eder. |
| [SetPriority](./setpriority/) | Bu koşullu biçimlendirme kuralının önceliği. Bu değer, whichformatın değerlendirilip işleneceğini belirlemek için kullanılır. Daha düşük sayısal değerler, thanhigher sayısal değerlere göre daha yüksek önceliğe sahiptir, burada '1' en yüksek önceliği temsil eder. |
| [GetStyle](./getstyle/) | Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar. |
| [SetStyle](./setstyle/) | Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar. |
| [GetType](./gettype/) | Koşullu biçim türünün durumunu alır ve ayarlar. |
| [SetType](./settype/) | Koşullu biçim türünün durumunu alır ve ayarlar. |
| [GetIconSet](./geticonset/) | Koşullu biçimlendirme'nin "IconSet" örneğini al.Varsayılan örneğin IconSetType'ı TrafficLights31'dir.Yalnızca type = IconSet için geçerlidir. |
| [GetDataBar](./getdatabar/) | Koşullu biçimlendirme'nin "DataBar" örneğini al.Varsayılan örneğin rengi mavidir.Yalnızca type = DataBar için geçerlidir. |
| [GetColorScale](./getcolorscale/) | Koşullu biçimlendirme'nin "ColorScale" örneğini al.Varsayılan örnek "green-yellow-red" 3ColorScale'dir.Yalnızca type = ColorScale için geçerlidir. |
| [GetTop10](./gettop10/) | Koşullu biçimlendirme'nin "Top10" örneğini al.Varsayılan örneğin kuralı, whosevalues en üst 10 aralığına düşen hücreleri vurgular.Yalnızca type = Top10 için geçerlidir. |
| [GetAboveAverage](./getaboveaverage/) | Koşullu biçimlendirme'nin "AboveAverage" örneğini al.Varsayılan örneğin kuralı, areabove ortalamanın üzerindeki hücreleri vurgular.Yalnızca type = AboveAverage için geçerlidir. |
| [GetText](./gettext/) | Bir "text contains" koşullu biçimlendirme kuralındaki metin değeri.Yalnızca type = containsText, notContainsText, beginsWith ve endsWith için geçerlidir.Varsayılan değer null'dur. |
| [SetText](./settext/) | Bir "text contains" koşullu biçimlendirme kuralındaki metin değeri.Yalnızca type = containsText, notContainsText, beginsWith ve endsWith için geçerlidir.Varsayılan değer null'dur. |
| [GetTimePeriod](./gettimeperiod/) | Bir "date occurrin" koşullu biçimlendirme kuralındaki geçerli zaman dilimi.Yalnızca type = timePeriod için geçerlidir.Varsayılan değer TimePeriodType.Today'tir. |
| [SetTimePeriod](./settimeperiod/) | Bir "date occurrin" koşullu biçimlendirme kuralındaki geçerli zaman dilimi.Yalnızca type = timePeriod için geçerlidir.Varsayılan değer TimePeriodType.Today'tir. |
