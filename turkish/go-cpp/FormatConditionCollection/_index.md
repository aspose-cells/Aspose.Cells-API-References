---
title: "FormatConditionCollection Sınıfı"
linktitle: "FormatConditionCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "FormatConditionCollection sınıfı. Go dilinde formatconditioncollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

Koşullu biçimlendirmeyi temsil eder. FormatConditions en fazla üç koşullu biçim içerebilir.

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | FormatConditions'a bir biçimlendirme koşulu ve etkilenmiş hücre aralığı ekler. FormatConditions en fazla üç koşullu biçim içerebilir. Koşullu biçimlendirme formüllerinde diğer sayfalara referans verilmesine izin verilmez. |
| [AddArea](./addarea/) | Koşullu biçimlendirilmiş bir hücre aralığı ekler. |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | Bir biçimlendirme koşulu ekler. |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | Bir biçim koşulu ekle. |
| [GetCount](./getcount/) | Koşulların sayısını alır. |
| [GetRangeCount](./getrangecount/) | Koşullu biçimlendirilmiş aralıkların sayısını alır. |
| [Get](./get/) | Biçimlendirme koşulunu indeks ile alır. |
| [GetCellArea](./getcellarea/) | Koşullu biçimlendirilmiş hücre aralığını indeks ile alır. |
| [RemoveArea_Int](./removearea_int/) | Koşullu biçimlendirilmiş hücre aralığını indeks ile kaldırır. |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | Aralıktaki koşullu biçimlendirmeyi kaldır. |
| [RemoveCondition](./removecondition/) | Biçimlendirme koşulunu indeks ile kaldırır. |
