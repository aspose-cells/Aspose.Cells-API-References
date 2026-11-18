---
title: "DataSorter Sınıfı"
linktitle: "DataSorter"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DataSorter sınıfı. Go'da datasorter'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/datasorter/
---

## DataSorter class

DataSorter için özet açıklama.

```go

type DataSorter struct  {
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
| [GetKeys](./getkeys/) | Veri sıralayıcısının anahtar listesini alır. |
| [Clear](./clear/) | Tüm ayarları temizle. |
| [GetHasHeaders](./gethasheaders/) | Aralığın başlık içerip içermediğini temsil eder. |
| [SetHasHeaders](./sethasheaders/) | Aralığın başlık içerip içermediğini temsil eder. |
| [AddKey_Int_SortOrder](./addkey_int_sortorder/) | Sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [AddColorKey](./addcolorkey/) | Renk sıralama anahtarını ekler. |
| [AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [GetKey1](./getkey1/) | İlk sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [SetKey1](./setkey1/) | İlk sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [GetOrder1](./getorder1/) | İlk anahtarın sıralama düzenini temsil eder. |
| [SetOrder1](./setorder1/) | İlk anahtarın sıralama düzenini temsil eder. |
| [GetKey2](./getkey2/) | İkinci sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [SetKey2](./setkey2/) | İkinci sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [GetOrder2](./getorder2/) | İkinci anahtarın sıralama düzenini temsil eder. |
| [SetOrder2](./setorder2/) | İkinci anahtarın sıralama düzenini temsil eder. |
| [GetKey3](./getkey3/) | Üçüncü sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [SetKey3](./setkey3/) | Üçüncü sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [GetOrder3](./getorder3/) | Üçüncü anahtarın sıralama düzenini temsil eder. |
| [SetOrder3](./setorder3/) | Üçüncü anahtarın sıralama düzenini temsil eder. |
| [GetSortLeftToRight](./getsortlefttoright/) | True, sıralama yönünün soldan sağa olduğunu ifade eder. False, sıralama yönünün üstten alta olduğunu ifade eder. Varsayılan değer false'tur. |
| [SetSortLeftToRight](./setsortlefttoright/) | True, sıralama yönünün soldan sağa olduğunu ifade eder. False, sıralama yönünün üstten alta olduğunu ifade eder. Varsayılan değer false'tur. |
| [GetCaseSensitive](./getcasesensitive/) | Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını alır ve ayarlar. |
| [SetCaseSensitive](./setcasesensitive/) | Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını alır ve ayarlar. |
| [GetSortAsNumber](./getsortasnumber/) | Bir sayıya benzeyen şeylerin sıralanıp sıralanmayacağını gösterir. |
| [SetSortAsNumber](./setsortasnumber/) | Bir sayıya benzeyen şeylerin sıralanıp sıralanmayacağını gösterir. |
| [Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | Alan verilerini sıralar. |
| [Sort_Cells_CellArea](./sort_cells_cellarea/) | Alan verilerini sırala. |
| [Sort](./sort/) | Aralıktaki verileri sırala. |
