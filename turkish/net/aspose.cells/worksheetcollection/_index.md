---
title: "Sınıf WorksheetCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WorksheetCollection sınıfı. Worksheet nesnelerinin bir koleksiyonunu kapsar."
type: docs
url: /tr/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Bir koleksiyonunu kapsar [`Worksheet`](../worksheet/) nesneleri.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | Elektronik tablo açıldığında etkin çalışma sayfasının dizinini temsil eder. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | Elektronik tablo açıldığında etkin çalışma sayfasının adını temsil eder. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | Elektronik tablonun tüm yerleşik belge özelliklerini temsil eden bir [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | Elektronik tablonun tüm özel belge özelliklerini temsil eden bir [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | Ana farklı biçimlendirme kayıtlarını alır. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | Bir çalışma kitabındaki harici bağlantıları temsil eder. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | MS Excel'de dosya açılırken tüm bağlantıların yenilenip yenilenmeyeceğini gösterir. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | Belirtilen dizindeki [`Worksheet`](../worksheet/) öğesini alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | Workbook dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır ve ayarlar. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | Tüm [`PivotCache`](../../aspose.cells.pivot/pivotcache/) öğelerini alır. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | Revizyon günlüklerini temsil eder. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | Tüm hassasiyet etiketlerini temsil eder. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | [`TableStyles`](./tablestyles/) nesnesini alır. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | İşlemeli yorum yazarlarının listesini alır. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | Görev bölmelerinin listesini alır. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | Görev bölmelerinin listesini alır. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | Çalışma kitabındaki XML haritalarını alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | Koleksiyona bir çalışma sayfası ekler. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | Koleksiyona bir çalışma sayfası ekler. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | Koleksiyona bir çalışma sayfası ekler. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | Bir grup çalışma sayfasını kopyalar. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | Tüm çalışma sayfalarını temizle. (2 yöntem) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | Pivot tablolarını elektronik tablodan temizler. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | Aralığın adresinden bir [`Range`](../range/) nesnesi oluşturur. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | Aralığın adresinden bir [`Range`](../range/) nesnesi oluşturur. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | Elektronik tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | Elektronik tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | Önceden tanımlanmış adla Range nesnesini alır. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | Önceden tanımlanmış ad veya tablonun adıyla [`Range`](../range/) alır |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | Kod adıyla çalışma sayfasını alır. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | Bir çalışma sayfası ekle. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | Bir çalışma sayfası ekle. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | (**Obsolete.**) Pivot kaynağıyla tüm pivot tablolarını ve grafikleri yenile. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | Excel dosyasındaki tüm PivotTables'ı yeniler. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Excel dosyasındaki tüm PivotTables'ı yeniler. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | Eklenti işlevini çalışma kitabına ekler |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | Eklenti işlevini çalışma kitabına ekler |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | Belirtilen indeksteki öğeyi kaldırır. (2 yöntem) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | Belirtilen adla öğeyi kaldırır. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | Workbook dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | Tanımlı adları sıralar. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | İki sayfayı değiştirir. |

### Örnekler

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // Koleksiyona yeni bir çalışma sayfası ekle
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // Var olan bir çalışma sayfasına indeksle eriş
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // Var olan bir çalışma sayfasına adla eriş
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // Etkin sayfayı ayarla
            worksheets.ActiveSheetIndex = newSheetIndex;

            // Etkin sayfanın adını ayarla
            worksheets.ActiveSheetName = "NewSheet";

            // Çalışma kitabındaki tüm pivot tablolarını yenile
            worksheets.RefreshAll();

            // Çalışma kitabından tüm pivot tablolarını temizle
            worksheets.ClearPivottables();

            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


