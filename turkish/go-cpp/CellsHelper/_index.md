---
title: "CellsHelper Sınıfı"
linktitle: "CellsHelper"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "CellsHelper sınıfı. Go'da cellshelper'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/cellshelper/
---

## CellsHelper class

Yardımcı işlevler sağlar.

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | Sayısal değerlerin çıktısı için varsayılan anlamlı basamak türünü alır ve ayarlar. Varsayılan değer SignificantDigitsType.G17'dir. |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | Sayısal değerlerin çıktısı için varsayılan anlamlı basamak türünü alır ve ayarlar. Varsayılan değer SignificantDigitsType.G17'dir. |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | Makinenin DPI değerini alır. |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | Makinenin DPI değerini alır. |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | Metnin genişliğini nokta biriminde al. |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | Sürüm numarasını al. |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | Hücrenin adını temel alarak satır ve sütun indekslerini alır. |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | Satır ve sütun indekslerine göre hücre adını alır. |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | Sütun indeksine göre sütun adını alır. |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | Sütun adına göre sütun indeksini alır. |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | Satır indeksine göre satır adını alır. |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | Satır adına göre satır indeksini alır. |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | Double değerini tarih saat değerine dönüştür. |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | Tarih saat değerini double değere dönüştür. |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | Başlangıç yolunu alır veya ayarlar; bu yol bazı dış formül referansları tarafından kullanılır. |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | Başlangıç yolunu alır veya ayarlar; bu yol bazı dış formül referansları tarafından kullanılır. |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | Alternatif başlangıç yolunu alır veya ayarlar; bu yol bazı dış formül referansları tarafından kullanılır. |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | Alternatif başlangıç yolunu alır veya ayarlar; bu yol bazı dış formül referansları tarafından kullanılır. |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | Kütüphane yolunu alır veya ayarlar; bu yol bazı dış formül referansları tarafından kullanılır. |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | Kütüphane yolunu alır veya ayarlar; bu yol bazı dış formül referansları tarafından kullanılır. |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | Çalışma kitabında kullanılan tüm renkleri alır. |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | Bazı büyük xls dosyalarını tek bir xls dosyasına birleştirir. |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü alır. |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | Veri önbelleği olarak kullanılabilecek geçici dosyalar için klasörü ayarlar. |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluk sınırı aşılırsa dize kırpılır ve geçersiz karakterler ' ' ile değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür. |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir ad oluşturur. Verilen sayfa adı Excel sayfa adı kurallarına uygunsa, onu döndürür. Aksi takdirde, uzunluk sınırı aşılırsa dize kırpılır ve geçersiz karakterler verilen karakterle değiştirilir, ardından yeniden oluşturulmuş dize değeri döndürülür. |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | Sayfa adının tek tırnak içinde olup olmayacağını gösterir |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | Bu özelliği, Azure, AWSLambda vb. gibi bir bulut platformunda çalışırken True olarak ayarlayın, |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | Bu özelliği, Azure, AWSLambda vb. gibi bir bulut platformunda çalışırken True olarak ayarlayın, |
