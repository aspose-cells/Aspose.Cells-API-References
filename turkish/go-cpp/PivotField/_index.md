---
title: "PivotField Class"
linktitle: "PivotField"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotField class. Go'da pivotfield'ı temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/pivotfield/
---

## PivotField class

Bir PivotTable raporundaki alanı temsil eder.

```go

type PivotField struct  {
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
| [GetPivotItems](./getpivotitems/) | Pivot alanının pivot öğelerini alır. |
| [GetMaxValue](./getmaxvalue/) | Bu alanın maksimum değerini alır. |
| [GetMinValue](./getminvalue/) | Bu alanın maksimum değerini alır. |
| [GetGroupSettings](./getgroupsettings/) | Pivot alanının grup ayarlarını alır. |
| [InitPivotItems](./initpivotitems/) | Pivot alanının pivot öğelerini başlatır. |
| [Group](./group/) | Alanı otomatik olarak gruplar. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Pivot alanını seçeneklerle gruplar. |
| [GroupBy](./groupby/) | Alanı özel olarak gruplar. |
| [Ungroup](./ungroup/) | Pivot alanının grubunu kaldırır. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | Pivot alanının tipine göre pivot filtresini alır |
| [GetFilters](./getfilters/) | Bu pivot alanına uygulanan tüm pivot filtrelerini alır. |
| [ClearFilter](./clearfilter/) | Bu pivot alanındaki filtre ayarını temizler. |
| [FilterTop10](./filtertop10/) | Veri pivot alanının değerlerine göre filtreler. |
| [FilterByValue](./filterbyvalue/) | Veri pivot alanının değerlerine göre filtreler. |
| [FilterByLabel](./filterbylabel/) | Satır veya sütun pivot alanının başlıklarına göre filtreler. |
| [FilterByDate](./filterbydate/) | Satır veya sütun pivot alanının tarih değerlerine göre filtreler. |
| [IsCalculatedField](./iscalculatedfield/) | Bu pivot alanının hesaplanmış alan olup olmadığını gösterir. |
| [GetFormula](./getformula/) | Hesaplanmış alanın formülünü alır. Yalnızca hesaplanmış alanlar için çalışır. |
| [IsValuesField](./isvaluesfield/) | Bu alanın değerler alanını temsil edip etmediğini gösterir. |
| [GetBaseIndex](./getbaseindex/) | Kaynak pivot alanlarındaki indeksi temsil eder. |
| [SetBaseIndex](./setbaseindex/) | Kaynak pivot alanlarındaki indeksi temsil eder. |
| [GetPosition](./getposition/) | Bölgedeki PivotField'ın indeksini temsil eder. |
| [GetRegionType](./getregiontype/) | Bu alanın görüntülendiği pivot tablo bölgesini belirtir. |
| [GetName](./getname/) | PivotField'ın adını temsil eder. |
| [SetName](./setname/) | PivotField'ın adını temsil eder. |
| [GetDisplayName](./getdisplayname/) | Pivot tablo görünümünde pivot alanın görüntü adını temsil eder. |
| [SetDisplayName](./setdisplayname/) | Pivot tablo görünümünde pivot alanın görüntü adını temsil eder. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Belirtilen alanın alt toplamının nasıl yapılacağını ayarlar. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Bu pivot alanı için belirtilen alt toplamın gösterilip gösterilmeyeceğini gösterir. |
| [GetSubtotals](./getsubtotals/) | Alan'ın alt toplamlarını alır veya ayarlar. Yalnızca Satır veya Sütun pivot alanı için. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Alan'ın alt toplamlarını alır veya ayarlar. Yalnızca Satır veya Sütun pivot alanı için. |
| [IsAutoSubtotals](./isautosubtotals/) | Belirtilen alanın otomatik alt toplamları gösterip göstermediğini gösterir. Varsayılan değer doğrudur. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | Belirtilen alanın otomatik alt toplamları gösterip göstermediğini gösterir. Varsayılan değer doğrudur. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | Belirtilen alanın satır bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Belirtilen alanın sütun bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | Belirtilen alanın sayfa bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. Varsayılan değer doğrudur. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | Bu pivot alanının PivotTable görünümünden kaldırılıp kaldırılamayacağını gösterir. Varsayılan değer doğrudur. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | Belirtilen alanın değerler bölgesine sürüklenip sürüklenemeyeceğini gösterir. Varsayılan değer doğrudur. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Sayfa alanında birden fazla öğenin seçilip seçilemeyeceğini gösterir. Varsayılan değer yanlıştır. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Sayfa alanında birden fazla öğenin seçilip seçilemeyeceğini gösterir. Varsayılan değer yanlıştır. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | Alanın etiketlerinin bölgede tekrarlanıp tekrarlanmayacağını gösterir. Varsayılan değer yanlıştır. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Alanın etiketlerinin bölgede tekrarlanıp tekrarlanmayacağını gösterir. Varsayılan değer yanlıştır. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Manuel filtrede alana yeni öğelerin dahil edilip edilmeyeceğini gösterir. Varsayılan değer yanlıştır. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Manuel filtrede alana yeni öğelerin dahil edilip edilmeyeceğini gösterir. Varsayılan değer yanlıştır. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Her öğeden sonra sayfa sonu eklenip eklenmeyeceğini gösterir. Varsayılan değer yanlıştır. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Her öğeden sonra sayfa sonu eklenip eklenmeyeceğini gösterir. Varsayılan değer yanlıştır. |
| [GetShowAllItems](./getshowallitems/) | PivotTable görünümünde tüm öğelerin gösterilip gösterilmeyeceğini, özet veri içermeseler bile belirtir. Varsayılan değer false'tur. |
| [SetShowAllItems](./setshowallitems/) | PivotTable görünümünde tüm öğelerin gösterilip gösterilmeyeceğini, özet veri içermeseler bile belirtir. Varsayılan değer false'tur. |
| [SortBy_SortOrder](./sortby_sortorder/) | Bu pivot alanını sıralar. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Bu pivot alanını sıralar. |
| [GetSortSetting](./getsortsetting/) | Otomatik sıralamanın tüm ayarlarını alır |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Bir pivot alanı için En İyi 10 Otomatik Göster ayarlarını alır. |
| [Top10AutoShow](./top10autoshow/) | Bu pivot alanı için En İyi 10 Otomatik Göster ayarlarını yapılandırır. |
| [GetFunction](./getfunction/) | Bu PivotTable veri alanını özetlemek için kullanılan işlevi temsil eder. |
| [SetFunction](./setfunction/) | Bu PivotTable veri alanını özetlemek için kullanılan işlevi temsil eder. |
| [ShowValuesAs](./showvaluesas/) | ShowDataAs hesaplaması kullanıldığında veri alanının değerlerini farklı bir görüntü biçiminde gösterir. |
| [GetShowValuesSetting](./getshowvaluessetting/) | ShowDataAs hesaplaması kullanıldığında değerlerin gösterilme ayarlarını alır. |
| [GetCurrentPageItem](./getcurrentpageitem/) | Veriyi filtrelemek için sayfa alanının şu anda seçili sayfa öğesini temsil eder. Yalnızca sayfa alanları için geçerlidir. |
| [SetCurrentPageItem](./setcurrentpageitem/) | Veriyi filtrelemek için sayfa alanının şu anda seçili sayfa öğesini temsil eder. Yalnızca sayfa alanları için geçerlidir. |
| [GetInsertBlankRow](./getinsertblankrow/) | Her öğeden sonra boş bir satır eklenip eklenmeyeceğini belirtir. Yalnızca satır alanları için. |
| [SetInsertBlankRow](./setinsertblankrow/) | Her öğeden sonra boş bir satır eklenip eklenmeyeceğini belirtir. Yalnızca satır alanları için. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | ShowInOutlineForm true olduğunda alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir, ardından |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | ShowInOutlineForm true olduğunda alt toplamların öğelerin üstünde mi yoksa altında mı gösterileceğini belirtir, ardından |
| [GetShowInOutlineForm](./getshowinoutlineform/) | Bu alanın Pivot Table görünümünde taslak biçiminde düzenlenip düzenlenmeyeceğini belirtir. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | Bu alanın Pivot Table görünümünde taslak biçiminde düzenlenip düzenlenmeyeceğini belirtir. |
| [GetNumber](./getnumber/) | Sayıların ve tarihlerin yerleşik görüntü biçimini temsil eder. |
| [SetNumber](./setnumber/) | Sayıların ve tarihlerin yerleşik görüntü biçimini temsil eder. |
| [Get_NumberFormat](./get_numberformat/) | Sayıların ve tarihlerin özel görüntü biçimini temsil eder. |
| [SetNumberFormat](./setnumberformat/) | Sayıların ve tarihlerin özel görüntü biçimini temsil eder. |
| [HideAllDetails](./hidealldetails/) | Tüm ayrıntıları gizler |
| [ShowAllDetails](./showalldetails/) | Tüm ayrıntıları göster |
| [GetItems](./getitems/) | Bu alandaki pivot öğelerinin tüm etiketlerini al. |
| [GetOriginalItems](./getoriginalitems/) | Orijinal temel öğeleri al; |
| [AddCalculatedItem](./addcalculateditem/) | Pivot alanına hesaplanmış bir formül öğesi ekle. |
| [GetShowCompact](./getshowcompact/) | Pivot Table görünümünde aynı sütunda bir sonraki alanın etiketlerinin gösterilip gösterilmeyeceğini belirtir |
| [SetShowCompact](./setshowcompact/) | Pivot Table görünümünde aynı sütunda bir sonraki alanın etiketlerinin gösterilip gösterilmeyeceğini belirtir |
