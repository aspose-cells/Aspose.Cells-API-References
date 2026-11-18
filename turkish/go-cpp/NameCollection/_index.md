---
title: "NameCollection Sınıfı"
linktitle: "NameCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "NameCollection sınıfı. Go'da namecollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/namecollection/
---

## NameCollection class

Elektronik tablo içindeki tüm <see cref=\"Name\"/> nesnelerinin bir koleksiyonunu temsil eder.

```go

type NameCollection struct  {
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
| [Add](./add/) | Yeni bir ad tanımlar. |
| [Get_Int](./get_int/) | Belirtilen indeksteki Name öğesini alır. |
| [Filter](./filter/) | Kapsama göre tanımlanan tüm adları alır. |
| [Get_String](./get_string/) | Belirtilen ada sahip Name öğesini alır. |
| [Remove_stringArray](./remove_stringarray/) | Bir dizi adı kaldır. |
| [Remove_String](./remove_string/) | Adı kaldır. |
| [RemoveAt](./removeat/) | Belirli indeksteki adı kaldır. |
| [Clear](./clear/) | Formüller ve veri kaynağı tarafından başvurulmayan tüm tanımlı adları kaldır. Tanımlı ad başvuruluyorsa, yalnızca Name.ReferTo'yu null olarak ayarlarız ve gizleriz. |
| [RemoveDuplicateNames](./removeduplicatenames/) | Yinelenen tanımlı adları kaldır |
| [Sort](./sort/) | Tanımlı adları sıralar. |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |
