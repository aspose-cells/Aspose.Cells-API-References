---
title: "WorksheetCollection Sınıfı"
linktitle: "WorksheetCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "WorksheetCollection sınıfı. Go'da worksheetcollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/worksheetcollection/
---

## WorksheetCollection class

<see cref=\"Worksheet\"/> nesnelerinin bir koleksiyonunu kapsüller.

```go

type WorksheetCollection struct  {
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
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Görev bölmelerinin listesini alır. |
| [GetWebExtensions](./getwebextensions/) | Görev bölmelerinin listesini alır. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | İş parçacıklı yorum yazarlarının listesini alır. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | MS Excel'de dosya açılırken tüm bağlantıların yenilenip yenilenmeyeceğini gösterir. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | MS Excel'de dosya açılırken tüm bağlantıların yenilenip yenilenmeyeceğini gösterir. |
| [CreateRange](./createrange/) | Aralığın adresinden bir Range nesnesi oluşturur. |
| [CreateUnionRange](./createunionrange/) | Aralığın adresinden bir Range nesnesi oluşturur. |
| [GetNames](./getnames/) | Elektronik tablo içindeki tüm Name nesnelerinin koleksiyonunu alır. |
| [Get_Int](./get_int/) | Belirtilen indeksteki Worksheet öğesini alır. |
| [Get_String](./get_string/) | Belirtilen ada sahip Worksheet öğesini alır. |
| [GetSheetByCodeName](./getsheetbycodename/) | Kod adıyla çalışma sayfasını alır. |
| [GetActiveSheetName](./getactivesheetname/) | Elektronik tablo açıldığında etkin çalışma sayfasının adını temsil eder. |
| [SetActiveSheetName](./setactivesheetname/) | Elektronik tablo açıldığında etkin çalışma sayfasının adını temsil eder. |
| [GetActiveSheetIndex](./getactivesheetindex/) | Elektronik tablo açıldığında etkin çalışma sayfasının indeksini temsil eder. |
| [SetActiveSheetIndex](./setactivesheetindex/) | Elektronik tablo açıldığında etkin çalışma sayfasının indeksini temsil eder. |
| [SortNames](./sortnames/) | Tanımlı adları sıralar. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | Bir çalışma sayfası ekle. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Bir çalışma sayfası ekle. |
| [Add_SheetType](./add_sheettype/) | Koleksiyona bir çalışma sayfası ekler. |
| [SwapSheet](./swapsheet/) | İki sayfayı değiştirir. |
| [Add](./add/) | Koleksiyona bir çalışma sayfası ekler. |
| [Add_String](./add_string/) | Koleksiyona bir çalışma sayfası ekler. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Eklenti işlevini çalışma kitabına ekler |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Eklenti işlevini çalışma kitabına ekler |
| [RemoveAt_String](./removeat_string/) | Belirtilen adla öğeyi kaldırır. |
| [RemoveAt_Int](./removeat_int/) | Belirtilen indeksteki öğeyi kaldırır. |
| [Clear](./clear/) | Tüm çalışma sayfalarını temizle. |
| [AddCopy_String](./addcopy_string/) | Koleksiyona bir çalışma sayfası ekler ve var olan bir çalışma sayfasından verileri kopyalar. |
| [AddCopy_Int](./addcopy_int/) | Koleksiyona bir çalışma sayfası ekler ve var olan bir çalışma sayfasından verileri kopyalar. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Bir grup çalışma sayfasını kopyala. |
| [GetDxfs](./getdxfs/) | Ana farklı biçimlendirme kayıtlarını alır. |
| [GetRangeByName_String](./getrangebyname_string/) | Önceden tanımlı adla Range nesnesini alır. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Önceden tanımlı adla veya tablonun adıyla Range'i alır |
| [GetNamedRanges](./getnamedranges/) | Elektronik tabloda tüm önceden tanımlı adlandırılmış aralıkları alır. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | Elektronik tabloda tüm önceden tanımlı adlandırılmış aralıkları alır. |
| [GetXmlMaps](./getxmlmaps/) | Çalışma kitabındaki XML haritalarını alır ve ayarlar. |
| [SetXmlMaps](./setxmlmaps/) | Çalışma kitabındaki XML haritalarını alır ve ayarlar. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Elektronik tabloyun tüm yerleşik belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Elektronik tabloyun tüm özel belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür. |
| [GetOleSize](./getolesize/) | Çalışma kitabı dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır ve ayarlar. |
| [SetOleSize_Object](./setolesize_object/) | Çalışma kitabı dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır ve ayarlar. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Çalışma kitabı dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar. |
| [GetExternalLinks](./getexternallinks/) | Bir çalışma kitabındaki dış bağlantıları temsil eder. |
| [GetPivotCaches](./getpivotcaches/) | Tüm PivotCache'i alır. |
| [GetTableStyles](./gettablestyles/) | TableStyles nesnesini alır. |
| [ClearPivottables](./clearpivottables/) | Elektronik tablodan pivot tabloları temizler. |
| [GetRevisionLogs](./getrevisionlogs/) | Revizyon günlüklerini temsil eder. |
| [RefreshPivotTables](./refreshpivottables/) | Excel dosyasındaki tüm PivotTables'i yeniler. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Excel dosyasındaki tüm PivotTables'i yeniler. |
| [GetSensitivityLabels](./getsensitivitylabels/) | Tüm hassasiyet etiketlerini temsil eder. |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |
