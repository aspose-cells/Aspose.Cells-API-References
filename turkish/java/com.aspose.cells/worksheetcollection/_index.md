---
title: "WorksheetCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

Bir [Worksheet](../../com.aspose.cells/worksheet) nesneleri koleksiyonunu kapsüller.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
 
         //Change the name of a worksheet
         sheets.get(0).setName("First Sheet");
 
         //Set the active sheet to the second worksheet
         sheets.setActiveSheetIndex(1);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add()](#add--) | Koleksiyona bir çalışma sayfası ekler. |
| [add(int type)](#add-int-) | Koleksiyona bir çalışma sayfası ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String sheetName)](#add-java.lang.String-) | Koleksiyona bir çalışma sayfası ekler. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Bir grup çalışma sayfasını kopyalar. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar. |
| [clear()](#clear--) | Tüm çalışma sayfalarını temizler. |
| [clearPivottables()](#clearPivottables--) | Elektronik tablodan pivot tabloları temizler. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Aralık adresinden bir [Range](../../com.aspose.cells/range) nesnesi oluşturur. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Aralık adresinden bir [Range](../../com.aspose.cells/range) nesnesi oluşturur. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [Worksheet](../../com.aspose.cells/worksheet) öğesini alır. |
| [get(String sheetName)](#get-java.lang.String-) | Belirtilen adla [Worksheet](../../com.aspose.cells/worksheet) öğesini alır. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder. |
| [getActiveSheetName()](#getActiveSheetName--) | Elektronik tablo açıldığında aktif çalışma sayfasının adını temsil eder. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm yerleşik belge özelliklerini temsil eder. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm özel belge özelliklerini temsil eder. |
| [getDxfs()](#getDxfs--) | Ana farklı biçimlendirme kayıtlarını alır. |
| [getExternalLinks()](#getExternalLinks--) | Bir çalışma kitabındaki dış bağlantıları temsil eder. |
| [getNamedRanges()](#getNamedRanges--) | Elektronik tablodaki tüm önceden tanımlı adlandırılmış aralıkları alır. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Elektronik tablodaki tüm önceden tanımlı adlandırılmış aralıkları alır. |
| [getNames()](#getNames--) | Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır. |
| [getOleSize()](#getOleSize--) | Workbook dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır. |
| [getPivotCaches()](#getPivotCaches--) | Tüm [PivotCache](../../com.aspose.cells/pivotcache) öğelerini alır. |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Önceden tanımlı adla Range nesnesini alır. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Önceden tanımlı ad veya tablonun adıyla [Range](../../com.aspose.cells/range) alır |
| [getRevisionLogs()](#getRevisionLogs--) | Revizyon günlüklerini temsil eder. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Tüm hassasiyet etiketlerini temsil eder. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Kod adıyla çalışma sayfasını alır. |
| [getTableStyles()](#getTableStyles--) | Alır [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) nesnesini. |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | İş parçacıklı yorum yazarlarının listesini alır. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Görev bölmelerinin listesini alır. |
| [getWebExtensions()](#getWebExtensions--) | Görev bölmelerinin listesini alır. |
| [getXmlMaps()](#getXmlMaps--) | Çalışma kitabındaki XML haritalarını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [insert(int index, int sheetType)](#insert-int-int-) | Bir çalışma sayfası ekleyin. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Bir çalışma sayfası ekleyin. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | MS Excel'de dosya açıldığında tüm bağlantıların yenilenip yenilenmeyeceğini gösterir. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Pivot kaynağıyla tüm pivot tabloları ve grafiklerini yenileyin. |
| [refreshPivotTables()](#refreshPivotTables--) | Excel dosyasındaki tüm PivotTable'ları yeniler. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Excel dosyasındaki tüm PivotTable'ları yeniler. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Eklenti işlevini çalışma kitabına ekler |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Eklenti işlevini çalışma kitabına ekler |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki öğeyi kaldırır. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Belirtilen isimdeki öğeyi kaldırır. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Elektronik tablo açıldığında aktif çalışma sayfasının adını temsil eder. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Çalışma kitabı dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Çalışma kitabı dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | MS Excel'de dosya açıldığında tüm bağlantıların yenilenip yenilenmeyeceğini gösterir. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Çalışma kitabındaki XML haritalarını ayarlar. |
| [sortNames()](#sortNames--) | Tanımlı adları sıralar. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | İki sayfayı değiştirir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Koleksiyona bir çalışma sayfası ekler.

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) nesne indeksi.
### add(int type) {#add-int-}
```
public int add(int type)
```


Koleksiyona bir çalışma sayfası ekler.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add(SheetType.CHART);
         	Cells cells = workbook.getWorksheets().get(0).getCells();
         	cells.get("c2").putValue(5000);
         	cells.get("c3").putValue(3000);
         	cells.get("c4").putValue(4000);
         	cells.get("c5").putValue(5000);
         	cells.get("c6").putValue(6000);
         	ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
         	int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
         	Chart chart = charts.get(chartIndex);
         	chart.getNSeries().add("Sheet1!C2:C6", true);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Çalışma sayfası türü. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) nesne indeksi.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


CollectionBase örneğine bir öğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğine eklenecek Nesne. |

**Returns:**
int - Yeni elemanın eklendiği konum.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


Koleksiyona bir çalışma sayfası ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Çalışma sayfası adı |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


Bir grup çalışma sayfasını kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | Kaynak çalışma sayfaları. |
| destSheetNames | java.lang.String[] | Kopyalanan sayfaların adları. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Kaynak çalışma sayfasının indeksi. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) nesne indeksi.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Kaynak çalışma sayfasının adı. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) nesne indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm çalışma sayfalarını temizler.

**Remarks**

Bir çalışma kitabı bir çalışma sayfası içermelidir.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


Elektronik tablodan pivot tabloları temizler.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Örneğin bu nesneyi içerip içermediğini döndürür

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | test nesnesi |

**Returns:**
boolean - Örneğin bu nesneyi içerip içermediği
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


Aralık adresinden bir [Range](../../com.aspose.cells/range) nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adres | java.lang.String | Aralığın adresi. |
| sheetIndex | int | Sayfa indeksi. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


Aralık adresinden bir [Range](../../com.aspose.cells/range) nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adres | java.lang.String | Aralığın adresi. |
| sheetIndex | int | Sayfa indeksi. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


Belirtilen indeksteki [Worksheet](../../com.aspose.cells/worksheet) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


Belirtilen adla [Worksheet](../../com.aspose.cells/worksheet) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Çalışma sayfası adı |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder.

**Remarks**

Sayfa indeksi sıfır tabanlıdır.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


Elektronik tablo açıldığında aktif çalışma sayfasının adını temsil eder.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm yerleşik belge özelliklerini temsil eder.

**Remarks**

Yerleşik belge özellikleri listesine yeni bir özellik eklenemez. Yalnızca bir yerleşik özelliği alabilir ve değerini değiştirebilirsiniz. Aşağıda yerleşik özelliklerin ad listesi verilmiştir:

Title

Konu

Yazar

Anahtar Kelimeler

Yorumlar

Şablon

Son Yazar

Revizyon Numarası

Uygulama Adı

Son Yazdırma Tarihi

Oluşturma Tarihi

Son Kaydetme Zamanı

Toplam Düzenleme Süresi

Sayfa Sayısı

Kelime Sayısı

Karakter Sayısı

Güvenlik

Kategori

Biçim

Yönetici

Şirket

Bayt Sayısı

Satır Sayısı

Paragraf Sayısı

Slayt Sayısı

Not Sayısı

Gizli Slayt Sayısı

Multimedya Klip Sayısı

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


CollectionBase örneğinde bulunan eleman sayısını alır.

**Returns:**
int - CollectionBase örneğinde bulunan eleman sayısı.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm özel belge özelliklerini temsil eder.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```


Ana farklı biçimlendirme kayıtlarını alır.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


Bir çalışma kitabındaki dış bağlantıları temsil eder.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


Elektronik tablodaki tüm önceden tanımlı adlandırılmış aralıkları alır.

**Returns:**
com.aspose.cells.Range[] - Range nesnelerinden oluşan bir dizi. Tanımlı Name'in referansı dışarıya yönlendirilmişse veya birden fazla aralık içeriyorsa, bu Name için hiçbir Range nesnesi döndürülmez.

Adlandırılmış aralık mevcut değilse null döndürür.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


Elektronik tablodaki tüm önceden tanımlı adlandırılmış aralıkları alır.

**Returns:**
com.aspose.cells.Range[] - Range nesnelerinden oluşan bir dizi.

Adlandırılmış aralık mevcut değilse null döndürür.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


Workbook dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır.

**Remarks**

Null, ole boyut ayarının olmadığını gösterir.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


Tüm [PivotCache](../../com.aspose.cells/pivotcache) öğelerini alır.

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


Önceden tanımlı adla Range nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rangeName | java.lang.String | Aralığın adı. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

Adlandırılmış aralık mevcut değilse null döndürür.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


Önceden tanımlı ad veya tablonun adıyla [Range](../../com.aspose.cells/range) alır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rangeName | java.lang.String | Aralığın adı veya tablonun adı. |
| currentSheetIndex | int | Sayfa indeksi. -1, global'ı temsil eder. |
| includeTable | boolean | Tüm tabloların kontrol edilip edilmediğini gösterir. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


Revizyon günlüklerini temsil eder.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


Tüm hassasiyet etiketlerini temsil eder.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


Kod adıyla çalışma sayfasını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| codeName | java.lang.String | Çalışma sayfası kod adı. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


Alır [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) nesnesini.

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


İş parçacıklı yorum yazarlarının listesini alır.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


Görev bölmelerinin listesini alır.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


Görev bölmelerinin listesini alır.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


Çalışma kitabındaki XML haritalarını alır.

**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


CollectionBase örneğindeki belirli bir öğenin dizinini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |

**Returns:**
int - Değer listede bulunursa dizini; aksi takdirde -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


Bir çalışma sayfası ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Sayfa indeksi |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Sayfa türü. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


Bir çalışma sayfası ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Sayfa indeksi |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Sayfa türü. |
| sheetName | java.lang.String | Sayfa adı. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


MS Excel'de dosya açıldığında tüm bağlantıların yenilenip yenilenmeyeceğini gösterir.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür.

**Returns:**
java.util.Iterator - CollectionBase örneği için bir iterator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Pivot kaynağıyla tüm pivot tabloları ve grafiklerini yenileyin.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Workbook.RefreshAll() metodunu kullanın. Bu metod, Nisan 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Excel dosyasındaki tüm PivotTable'ları yeniler.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Excel dosyasındaki tüm PivotTable'ları yeniler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Pivot tablolarının veri kaynağını yenileme seçeneği. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


Eklenti işlevini çalışma kitabına ekler

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| id | int | Eklenti fonksiyonlarını içeren verinin ID'si, aynı eklenti dosyası için [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) metodunun ilk çağrısı ile elde edilebilir. |
| functionName | java.lang.String | eklentinin fonksiyon adı |

**Returns:**
java.lang.String - Eklenti fonksiyonlarını içeren eklenti dosyasının URL'si
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


Eklenti işlevini çalışma kitabına ekler

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| addInFile | java.lang.String | eklentinin fonksiyonlarını içeren dosya |
| functionName | java.lang.String | eklentinin fonksiyon adı |
| lib | boolean | verilen eklenti dosyasının Workbook Add-In kitaplığının dizininde veya alt dizininde olup olmadığını belirler. Bu bayrak, verilen addInFile göreceli bir yol olduğunda etkili olur ve fark yaratır: true, yolun Add-In kitaplığına göreceli olduğunu, false ise yolun bu Workbook'a göreceli olduğunu gösterir. |

**Returns:**
int - Verilen eklenti işlevini içeren verinin kimliği.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen indeksteki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak öğenin indeks değeri. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Belirtilen isimdeki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Kaldırılacak öğenin adı. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder.

**Remarks**

Sayfa indeksi sıfır tabanlıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


Elektronik tablo açıldığında aktif çalışma sayfasının adını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


Çalışma kitabı dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar.

**Remarks**

Bu yöntem genellikle ppt dosyasında veya doc dosyasında görüntü boyutunu ayarlamak için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satır indeksi. |
| endRow | int | Bitiş satır indeksi. |
| startColumn | int | Başlangıç sütun indeksi. |
| endColumn | int | Bitiş sütun indeksi. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


Çalışma kitabı dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar.

**Remarks**

Null, ole boyut ayarının olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


MS Excel'de dosya açıldığında tüm bağlantıların yenilenip yenilenmeyeceğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


Çalışma kitabındaki XML haritalarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


Tanımlı adları sıralar.

**Remarks**

Excel dosyasında çok sayıda adlandırılmış aralık oluşturursanız, lütfen bu yöntemi tüm adlandırılmış aralıklar oluşturulduktan ve kaydetmeden önce çağırın.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


İki sayfayı değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex1 | int | İlk çalışma sayfası. |
| sheetIndex2 | int | İkinci çalışma sayfası. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

