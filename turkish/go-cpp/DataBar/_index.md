---
title: "DataBar Sınıfı"
linktitle: "DataBar"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DataBar sınıfı. Go dilinde databar'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/databar/
---

## DataBar class

DataBar koşullu biçimlendirme kuralını açıklar. Bu koşullu biçimlendirme kuralı hücre aralığında kademeli bir veri çubuğu gösterir.

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | Koşullu biçimlendirme ile veri çubukları olarak kullanılan hücrelerin ekseninin rengini alır. |
| [SetAxisColor](./setaxiscolor/) | Koşullu biçimlendirme ile veri çubukları olarak kullanılan hücrelerin ekseninin rengini alır. |
| [GetAxisPosition](./getaxisposition/) | Koşullu biçimlendirme kuralı ile belirtilen veri çubuklarının eksen konumunu alır veya ayarlar. |
| [SetAxisPosition](./setaxisposition/) | Koşullu biçimlendirme kuralı ile belirtilen veri çubuklarının eksen konumunu alır veya ayarlar. |
| [GetBarFillType](./getbarfilltype/) | Bir veri çubuğunun renk ile nasıl doldurulduğunu alır veya ayarlar. |
| [SetBarFillType](./setbarfilltype/) | Bir veri çubuğunun renk ile nasıl doldurulduğunu alır veya ayarlar. |
| [GetDirection](./getdirection/) | Veri çubuğunun görüntülendiği yönü alır veya ayarlar. |
| [SetDirection](./setdirection/) | Veri çubuğunun görüntülendiği yönü alır veya ayarlar. |
| [GetBarBorder](./getbarborder/) | Bir veri çubuğunun kenarlığını belirten nesneyi alır. |
| [GetNegativeBarFormat](./getnegativebarformat/) | Bir veri çubuğu koşullu biçimlendirme kuralı ile ilişkili NegativeBarFormat nesnesini alır. |
| [GetMinCfvo](./getmincfvo/) | Bu DataBar'ın minimum değer nesnesini al veya ayarla. Null veya FormatConditionValueType.Max tipinde CFValueObject atanamaz. |
| [GetMaxCfvo](./getmaxcfvo/) | Bu DataBar'ın maksimum değer nesnesini al veya ayarla. Null veya FormatConditionValueType.Min tipinde CFValueObject atanamaz. |
| [GetColor](./getcolor/) | Bu DataBar'ın Rengini al veya ayarla. |
| [SetColor](./setcolor/) | Bu DataBar'ın Rengini al veya ayarla. |
| [GetMinLength](./getminlength/) | Veri çubuğunun minimum uzunluğunu temsil eder. |
| [SetMinLength](./setminlength/) | Veri çubuğunun minimum uzunluğunu temsil eder. |
| [GetMaxLength](./getmaxlength/) | Veri çubuğunun maksimum uzunluğunu temsil eder. |
| [SetMaxLength](./setmaxlength/) | Veri çubuğunun maksimum uzunluğunu temsil eder. |
| [GetShowValue](./getshowvalue/) | Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı al veya ayarla. Varsayılan değer doğrudur. |
| [SetShowValue](./setshowvalue/) | Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı al veya ayarla. Varsayılan değer doğrudur. |
| [ToImage](./toimage/) | Hücredeki veri çubuğunu görüntü bayt dizisine render eder. |
