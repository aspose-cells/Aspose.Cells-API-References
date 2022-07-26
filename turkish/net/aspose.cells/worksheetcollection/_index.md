---
title: WorksheetCollection
second_title: Aspose.Cells for .NET API Referansı
description: Bir koleksiyonu kapsüllerWorksheet./worksheet nesneler.
type: docs
weight: 6520
url: /tr/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Bir koleksiyonu kapsüller[`Worksheet`](../worksheet) nesneler.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Elektronik tablo açıldığında etkin çalışma sayfasının dizinini temsil eder. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Elektronik tablo açıldığında etkin çalışma sayfasının adını temsil eder. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Bir döndürür[`DocumentProperty`](../../aspose.cells.properties/documentproperty)elektronik tablonun tüm yerleşik belge özelliklerini temsil eden koleksiyon. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Bir döndürür[`DocumentProperty`](../../aspose.cells.properties/documentproperty) elektronik tablonun tüm özel belge özelliklerini temsil eden koleksiyon. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Ana diferansiyel biçimlendirme kayıtlarını alır. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Bir çalışma kitabındaki harici bağlantıları temsil eder. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Dosyayı MS Excel'de açarken tüm bağlantıların yenilenip yenilenmediğini gösterir. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | [`Worksheet`](../worksheet) belirtilen dizindeki öğe. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Elektronik tablodaki tüm Ad nesnelerinin koleksiyonunu alır. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Çalışma Kitabı dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır ve ayarlar. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Revizyon günlüklerini temsil eder. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | Alır[`TableStyles`](./tablestyles) nesne. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Dizili yorum yazarlarının listesini alır. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Görev bölmelerinin listesini alır. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Görev bölmelerinin listesini alır. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Çalışma kitabındaki XML eşlemelerini alır ve ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Koleksiyona bir çalışma sayfası ekler. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Koleksiyona bir çalışma sayfası ekler. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Koleksiyona bir çalışma sayfası ekler. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından veri kopyalar. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından veri kopyalar. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Tüm çalışma sayfalarını temizleyin. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Özet tabloları elektronik tablodan temizler. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Bir[`Range`](../range) aralığının bir adresinden nesne. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Bir[`Range`](../range) aralığının bir adresinden nesne. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | E-tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | E-tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Range nesnesini önceden tanımlanmış ada göre alır. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | Alır[`Range`](../range) önceden tanımlanmış ad veya tablo adına göre |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Çalışma sayfasını kod adına göre alır. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Bir çalışma sayfası ekleyin. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Bir çalışma sayfası ekleyin. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | WorksheetCollection'daki tüm PivotTable'ları yeniler. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Çalışma kitabına eklenti işlevi ekler |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Çalışma kitabına eklenti işlevi ekler |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Belirtilen dizindeki öğeyi kaldırır. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Belirtilen addaki öğeyi kaldırır. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Çalışma Kitabı dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Tanımlanan adları sıralar. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | İki sayfayı değiştirir. |

### Örnekler

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Çalışma sayfası ekle
sheets.Add();

//Çalışma sayfasının adını değiştir
sheets[0].Name = "First Sheet";

//Etkin sayfayı ikinci çalışma sayfasına ayarla
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Çalışma sayfası ekle
sheets.Add()

'Çalışma sayfasının adını değiştirme
sheets(0).Name = "First Sheet"

'Etkin sayfayı ikinci çalışma sayfasına ayarlayın
sheets.ActiveSheetIndex = 1
```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
