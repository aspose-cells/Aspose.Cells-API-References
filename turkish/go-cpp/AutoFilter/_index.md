---
title: "AutoFilter Sınıfı"
linktitle: "AutoFilter"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "AutoFilter sınıfı. Go'da otomatik filtreyi temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/autofilter/
---

## AutoFilter class

Belirtilen çalışma sayfası için otomatik filtrelemeyi temsil eder.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | Veri sıralayıcıyı alır. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar. |
| [GetCellArea](./getcellarea/) | Bu AutoFilter'ın uygulandığı CellArea'yı alır. |
| [GetCellArea_Bool](./getcellarea_bool/) | Belirtilen AutoFilter'ın uygulandığı Aspose.Cells.CellArea'yı alır. |
| [GetRange](./getrange/) | Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder. |
| [SetRange_String](./setrange_string/) | Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder. |
| [AddFilter](./addfilter/) | Bir filtre sütunu için filtre ekler. |
| [AddDateFilter](./adddatefilter/) | Bir tarih filtresi ekler. |
| [RemoveDateFilter](./removedatefilter/) | Bir tarih filtresini kaldırır. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | Bir filtre sütunu için filtreyi kaldırır. |
| [Filter](./filter/) | Belirtilen ölçütlerle bir listeyi filtreler. |
| [FilterTop10](./filtertop10/) | Listedeki ilk 10 öğeyi filtrele |
| [Dynamic_Filter](./dynamic_filter/) | Dinamik bir filtre ekler. |
| [AddFontColorFilter](./addfontcolorfilter/) | Yazı tipi rengi filtresi ekler. |
| [AddFillColorFilter](./addfillcolorfilter/) | Dolgu rengi filtresi ekler. |
| [AddIconFilter](./addiconfilter/) | Simge filtresi ekler. |
| [MatchBlanks](./matchblanks/) | Listedeki tüm boş hücreleri eşleştir. |
| [MatchNonBlanks](./matchnonblanks/) | Listedeki tüm boş olmayan hücreleri eşleştir. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Özel bir ölçütle bir listeyi filtreler. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Bir listeyi özel kriterlerle filtreler. |
| [ShowAll](./showall/) | Tüm satırların gizlenmesini kaldır. |
| [RemoveFilter_Int](./removefilter_int/) | Belirli filtreyi kaldır. |
| [Refresh](./refresh/) | Satırları gizlemek veya göstermek için otomatik filtreleri yenile |
| [Refresh_Bool](./refresh_bool/) | Tüm gizli satırların indekslerini alır. |
| [GetShowFilterButton](./getshowfilterbutton/) | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [SetShowFilterButton](./setshowfilterbutton/) | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [GetFilterColumns](./getfiltercolumns/) | Filtre sütunlarının koleksiyonunu alır. |
