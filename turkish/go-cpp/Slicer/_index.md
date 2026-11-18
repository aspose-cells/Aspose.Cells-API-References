---
title: "Slicer Sınıfı"
linktitle: "Slicer"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Slicer sınıfı. Go'da slicer'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/slicer/
---

## Slicer class

Slicer Görünümü'nün özet açıklaması

```go

type Slicer struct  {
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
| [GetSortOrderType](./getsortordertype/) | Öğeleri sıralama türünü belirtir. |
| [SetSortOrderType](./setsortordertype/) | Öğeleri sıralama türünü belirtir. |
| [GetShowMissing](./getshowmissing/) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [SetShowMissing](./setshowmissing/) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | Veri kaynağından silinen öğelerin gösterilip gösterilmeyeceğini belirtir. |
| [GetShowAllItems](./getshowallitems/) | Veri yoksa veya öğeler silinmiş olsa bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. Varsayılan değer true'dur; |
| [SetShowAllItems](./setshowallitems/) | Veri yoksa veya öğeler silinmiş olsa bile tüm öğelerin gösterilip gösterilmeyeceğini belirtir. Varsayılan değer true'dur; |
| [AddPivotConnection](./addpivotconnection/) | PivotTable bağlantısı ekler. |
| [RemovePivotConnection](./removepivotconnection/) | PivotTable bağlantısını kaldırır. |
| [GetLockedPosition](./getlockedposition/) | Belirtilen slicer'ın kullanıcı arayüzü kullanılarak taşınıp yeniden boyutlandırılıp boyutlandırılamayacağını belirtir. |
| [SetLockedPosition](./setlockedposition/) | Belirtilen slicer'ın kullanıcı arayüzü kullanılarak taşınıp yeniden boyutlandırılıp boyutlandırılamayacağını belirtir. |
| [Refresh](./refresh/) | İlgili pivot tablolarından slicer öğelerini yeniliyor. |
| [GetShape](./getshape/) | Belirtilen slicer ile ilişkili Shape nesnesini döndürür. Salt okunur. |
| [GetSlicerCache](./getslicercache/) | Slicer ile ilişkili SlicerCache nesnesini döndürür. Salt okunur. |
| [GetWorksheet](./getworksheet/) | Bu slicer'ı içeren Worksheet nesnesini döndürür. Salt okunur. |
| [GetStyleType](./getstyletype/) | Yerleşik slicer stilinin türünü belirtin. Varsayılan tür SlicerStyleLight1'dir. |
| [SetStyleType](./setstyletype/) | Yerleşik slicer stilinin türünü belirtin. Varsayılan tür SlicerStyleLight1'dir. |
| [GetName](./getname/) | Belirtilen slicer'ın adını döndürür veya ayarlar |
| [SetName](./setname/) | Belirtilen slicer'ın adını döndürür veya ayarlar |
| [GetCaption](./getcaption/) | Belirtilen slicer'ın başlığını döndürür veya ayarlar. |
| [SetCaption](./setcaption/) | Belirtilen slicer'ın başlığını döndürür veya ayarlar. |
| [GetFirstItemIndex](./getfirstitemindex/) | İlk slicer öğesinin sıfır tabanlı dizinini belirtir. |
| [SetFirstItemIndex](./setfirstitemindex/) | İlk slicer öğesinin sıfır tabanlı dizinini belirtir. |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | Seçili filtre etiketlerini kaldır. |
| [ClearFilter](./clearfilter/) | Filtreleri kaldır |
| [GetShowCaption](./getshowcaption/) | Slicer başlığının görünür olup olmadığını belirtir. Varsayılan değer true'dur |
| [SetShowCaption](./setshowcaption/) | Slicer başlığının görünür olup olmadığını belirtir. Varsayılan değer true'dur |
| [GetNumberOfColumns](./getnumberofcolumns/) | Slicer'daki sütun sayısını döndürür veya ayarlar. Varsayılan değer 1'dir. |
| [SetNumberOfColumns](./setnumberofcolumns/) | Slicer'daki sütun sayısını döndürür veya ayarlar. Varsayılan değer 1'dir. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | Slicer'daki her sütunun genişliğini piksel biriminde alır veya ayarlar. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | Slicer'daki her sütunun genişliğini piksel biriminde alır veya ayarlar. |
| [GetColumnWidth](./getcolumnwidth/) | Slicer'daki her sütunun genişliğini nokta biriminde döndürür veya ayarlar. |
| [SetColumnWidth](./setcolumnwidth/) | Slicer'daki her sütunun genişliğini nokta biriminde döndürür veya ayarlar. |
| [GetRowHeightPixel](./getrowheightpixel/) | Belirtilen slicer'daki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar. |
| [SetRowHeightPixel](./setrowheightpixel/) | Belirtilen slicer'daki her satırın yüksekliğini piksel biriminde döndürür veya ayarlar. |
| [GetRowHeight](./getrowheight/) | Belirtilen slicer'daki her satırın yüksekliğini nokta biriminde döndürür veya ayarlar. |
| [SetRowHeight](./setrowheight/) | Belirtilen slicer'daki her satırın yüksekliğini nokta biriminde döndürür veya ayarlar. |
