---
title: "ConditionalFormattingValue Sınıfı"
linktitle: "ConditionalFormattingValue"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ConditionalFormattingValue sınıfı. Go'da conditionalformattingvalue'yi temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Bir gradient ölçeği, dataBar veya iconSet içindeki ara nokta değerlerini açıklar.

```go

type ConditionalFormattingValue struct  {
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
| [GetValue](./getvalue/) | Bu koşullu biçimlendirme değeri nesnesinin değerini alın veya ayarlayın. Tip ile birlikte kullanılmalıdır. |
| [SetValue](./setvalue/) | Bu koşullu biçimlendirme değeri nesnesinin değerini alın veya ayarlayın. Tip ile birlikte kullanılmalıdır. |
| [GetType](./gettype/) | Bu koşullu biçimlendirme değeri nesnesinin tipini alın veya ayarlayın. Tipi FormatConditionValueType.Min veya FormatConditionValueType.Max olarak ayarlamak, \"Value\" değerini otomatik olarak null yapar. |
| [SetType](./settype/) | Bu koşullu biçimlendirme değeri nesnesinin tipini alın veya ayarlayın. Tipi FormatConditionValueType.Min veya FormatConditionValueType.Max olarak ayarlamak, \"Value\" değerini otomatik olarak null yapar. |
| [IsGTE](./isgte/) | Büyük veya Eşit bayrağını alın veya ayarlayın. Yalnızca simge setleri için kullanılır, bu eşik değerinin büyük veya eşit operatörünü kullanıp kullanmayacağını belirler. 'false' değeri, 'büyük' operatörünün kullanıldığını, 'büyük veya eşit' yerine gösterir. Varsayılan değer true'tır. |
| [SetIsGTE](./setisgte/) | Büyük veya Eşit bayrağını alın veya ayarlayın. Yalnızca simge setleri için kullanılır, bu eşik değerinin büyük veya eşit operatörünü kullanıp kullanmayacağını belirler. 'false' değeri, 'büyük' operatörünün kullanıldığını, 'büyük veya eşit' yerine gösterir. Varsayılan değer true'tır. |
