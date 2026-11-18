---
title: "PivotTableCollection Sınıfı"
linktitle: "PivotTableCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotTableCollection sınıfı. Go'da pivottablecollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivottablecollection/
---

## PivotTableCollection class

Belirtilen çalışma sayfasındaki tüm PivotTable nesnelerinin koleksiyonunu temsil eder.

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | Yönetilmeyen kaynakları serbest bırakma, bırakma veya sıfırlama ile ilgili uygulama tanımlı görevleri yürütür. |
| [Add_String_Int_Int](./add_string_int_int/) | Belirtilen çalışma sayfası satır ve sütun konumunda varsayılan seçeneklerle yeni bir PivotTable ekler. |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | Eski Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler. |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | Yeni bir PivotTable ekler. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Başka bir PivotTable'a dayalı yeni bir PivotTable ekler. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Başka bir PivotTable'a dayalı yeni bir PivotTable ekler. |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | Veri kaynağı olarak birden fazla konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler. |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | Veri kaynağı olarak birden fazla konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler. |
| [Get_Int](./get_int/) | PivotTable raporunu indeksle alır. |
| [Get_String](./get_string/) | PivotTable raporunu adla alır. |
| [Get_Int_Int](./get_int_int/) | PivotTable raporunu konumla alır. |
| [Clear](./clear/) | Tüm pivot tabloları temizler. |
| [Remove_PivotTable](./remove_pivottable/) | Belirtilen PivotTable'ı siler ve PivotTable verilerini siler |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | Belirtilen PivotTable'ı siler |
| [RemoveAt_Int](./removeat_int/) | Belirtilen indeksdeki PivotTable'ı siler ve PivotTable verilerini siler |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | Belirtilen indeksdeki PivotTable'ı siler |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |
