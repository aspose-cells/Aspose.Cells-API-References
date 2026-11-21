---
title: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Yerleşik belge özelliklerinin bir koleksiyonu."
type: docs
url: /tr/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

Yerleşik belge özelliklerinin bir koleksiyonu.

**Remarks**

Nesnelere adlarıyla (indeksleyici kullanarak) ve uygun tiplerde değerler döndüren bir dizi tiplenmiş özellik aracılığıyla erişim sağlar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [contains(String name)](#contains-java.lang.String-) | Belirtilen ada sahip bir özellik koleksiyonda mevcutsa true döndürür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | İndeks ile bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür. |
| [get(String name)](#get-java.lang.String-) | Özelliğin adıyla bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür. |
| [getAuthor()](#getAuthor--) | Belgenin yazarının adını alır. |
| [getBytes()](#getBytes--) | Belgedeki bayt sayısının bir tahminini temsil eder. |
| [getCategory()](#getCategory--) | Belgenin kategorisini alır. |
| [getCharacters()](#getCharacters--) | Belgedeki karakter sayısının bir tahminini temsil eder. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | Belgedeki karakter (boşluklar dahil) sayısının bir tahminini temsil eder. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Belge yorumlarını alır. |
| [getCompany()](#getCompany--) | Şirket özelliğini alır. |
| [getContentStatus()](#getContentStatus--) | Belgenin içerik durumunu alır. |
| [getContentType()](#getContentType--) | Belgenin içerik türünü alır. |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getCreatedTime()](#getCreatedTime--) | Belgenin oluşturulma tarihini yerel saat diliminde alır. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | Belgenin oluşturulma evrensel zamanını alır. |
| [getDocumentVersion()](#getDocumentVersion--) | Dosyanın sürümünü temsil eder. |
| [getHyperlinkBase()](#getHyperlinkBase--) | hyperlinkbase özelliğini alır. |
| [getKeywords()](#getKeywords--) | Belge anahtar kelimelerini alır. |
| [getLanguage()](#getLanguage--) | Belgenin dilini alır. |
| [getLastPrinted()](#getLastPrinted--) | Belgenin en son yazdırıldığı tarihi yerel saat diliminde alır. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | Belgenin en son yazdırıldığı evrensel zamanı alır. |
| [getLastSavedBy()](#getLastSavedBy--) | Son yazarın adını alır. |
| [getLastSavedTime()](#getLastSavedTime--) | Son kaydetme zamanını yerel saat diliminde alır. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | Son kaydetmenin evrensel zamanını alır. |
| [getLines()](#getLines--) | Belge içindeki satır sayısının tahmini bir temsilidir. |
| [getLinksUpToDate()](#getLinksUpToDate--) | Belgedeki köprülerin güncel olup olmadığını gösterir. |
| [getManager()](#getManager--) | Yönetici özelliğini alır. |
| [getNameOfApplication()](#getNameOfApplication--) | Uygulamanın adını alır. |
| [getPages()](#getPages--) | Belge içindeki sayfa sayısının tahmini bir temsilidir. |
| [getParagraphs()](#getParagraphs--) | Belge içindeki paragraf sayısının tahmini bir temsilidir. |
| [getRevisionNumber()](#getRevisionNumber--) | Belge revizyon numarasını alır. |
| [getScaleCrop()](#getScaleCrop--) | Belge küçük resminin görüntüleme modunu gösterir. |
| [getSubject()](#getSubject--) | Belgenin konusunu alır. |
| [getTemplate()](#getTemplate--) | Belge şablonunun bilgi adını alır. |
| [getTitle()](#getTitle--) | Belgenin başlığını alır. |
| [getTotalEditingTime()](#getTotalEditingTime--) | Toplam düzenleme süresini dakikalar cinsinden alır. |
| [getVersion()](#getVersion--) | Belgeyi oluşturan uygulamanın sürüm numarasını temsil eder. |
| [getWords()](#getWords--) | Belge içindeki kelime sayısının tahmini bir temsilidir. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Adına göre bir özelliğin indeksini alır. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Belirtilen ada sahip bir özelliği koleksiyondan kaldırır. |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki bir özelliği kaldırır. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Belgenin yazarının adını ayarlar. |
| [setBytes(int value)](#setBytes-int-) | Belgedeki bayt sayısının bir tahminini temsil eder. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Belgenin kategorisini ayarlar. |
| [setCharacters(int value)](#setCharacters-int-) | Belgedeki karakter sayısının bir tahminini temsil eder. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | Belgedeki karakter (boşluklar dahil) sayısının bir tahminini temsil eder. |
| [setComments(String value)](#setComments-java.lang.String-) | Belge yorumlarını ayarlar. |
| [setCompany(String value)](#setCompany-java.lang.String-) | Şirket özelliğini ayarlar. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | Belgenin içerik durumunu ayarlar. |
| [setContentType(String value)](#setContentType-java.lang.String-) | Belgenin içerik türünü ayarlar. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Belgenin oluşturulma tarihini yerel saat diliminde ayarlar. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | Belgenin oluşturulma evrensel zamanını ayarlar. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | Dosyanın sürümünü temsil eder. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | Köprü tabanı özelliğini ayarlar. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | Belge anahtar kelimelerini ayarlar. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | Belgenin dilini ayarlar. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | Belgenin en son yazdırıldığı tarihi yerel saat diliminde ayarlar. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | Belgenin en son yazdırıldığı evrensel zamanı ayarlar. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | Son yazarın adını ayarlar. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | En son kaydetmenin zamanını yerel saat diliminde ayarlar. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | En son kaydetmenin evrensel zamanını ayarlar. |
| [setLines(int value)](#setLines-int-) | Belge içindeki satır sayısının tahmini bir temsilidir. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | Belgedeki köprülerin güncel olup olmadığını gösterir. |
| [setManager(String value)](#setManager-java.lang.String-) | Yönetici özelliğini ayarlar. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | Uygulamanın adını ayarlar. |
| [setPages(int value)](#setPages-int-) | Belge içindeki sayfa sayısının tahmini bir temsilidir. |
| [setParagraphs(int value)](#setParagraphs-int-) | Belge içindeki paragraf sayısının tahmini bir temsilidir. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | Belge revizyon numarasını ayarlar. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | Belge küçük resminin görüntüleme modunu gösterir. |
| [setSubject(String value)](#setSubject-java.lang.String-) | Belgenin konusunu ayarlar. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | Belge şablonunun bilgilendirici adını ayarlar. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Belgenin başlığını ayarlar. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | Toplam düzenleme süresini dakikalar cinsinden ayarlar. |
| [setVersion(String value)](#setVersion-java.lang.String-) | Belgeyi oluşturan uygulamanın sürüm numarasını temsil eder. |
| [setWords(int value)](#setWords-int-) | Belge içindeki kelime sayısının tahmini bir temsilidir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### clear() {#clear--}
```
public void clear()
```


CollectionBase örneğinden tüm nesneleri kaldırır.

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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Belirtilen ada sahip bir özellik koleksiyonda mevcutsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin büyük/küçük harfe duyarsız adı. |

**Returns:**
boolean - Özellik koleksiyonda mevcutsa true; aksi takdirde false.
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
public DocumentProperty get(int index)
```


İndeks ile bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Alınacak [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesinin sıfır tabanlı indeksi. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Özelliğin adıyla bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür.

**Remarks**

Özelliklerin dize adları, . içinde mevcut olan tiplenmiş özelliklerin adlarıyla eşleşir.

Eğer belgede bulunmayan bir özelliği talep ederseniz, ancak özelliğin adı geçerli bir yerleşik ad olarak tanınıyorsa, yeni bir  oluşturulur, koleksiyona eklenir ve döndürülür. Yeni oluşturulan özelliğe varsayılan bir değer atanır (boş dize, sıfır, false veya DateTime.MinValue, yerleşik özelliğin türüne bağlı olarak).

Eğer belgede bulunmayan bir özelliği talep eder ve ad yerleşik bir ad olarak tanınmazsa, null döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Alınacak özelliğin büyük/küçük harfe duyarsız adı. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Belgenin yazarının adını alır.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


Belgedeki bayt sayısının bir tahminini temsil eder.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


Belgenin kategorisini alır.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


Belgedeki karakter sayısının bir tahminini temsil eder.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


Belgedeki karakter (boşluklar dahil) sayısının bir tahminini temsil eder.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


Belge yorumlarını alır.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


Şirket özelliğini alır.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


Belgenin içerik durumunu alır.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


Belgenin içerik türünü alır.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


CollectionBase örneğinde bulunan eleman sayısını alır.

**Returns:**
int - CollectionBase örneğinde bulunan eleman sayısı.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Belgenin oluşturulma tarihini yerel saat diliminde alır.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


Belgenin oluşturulma evrensel zamanını alır.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


Dosyanın sürümünü temsil eder.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


hyperlinkbase özelliğini alır.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


Belge anahtar kelimelerini alır.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


Belgenin dilini alır.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


Belgenin en son yazdırıldığı tarihi yerel saat diliminde alır.

**Remarks**

Belge hiç yazdırılmadıysa, bu özellik DateTime.MinValue döndürecektir.

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


Belgenin en son yazdırıldığı evrensel zamanı alır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


Son yazarın adını alır.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


Son kaydetme zamanını yerel saat diliminde alır.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


Son kaydetmenin evrensel zamanını alır.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


Belge içindeki satır sayısının tahmini bir temsilidir.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


Belgedeki köprülerin güncel olup olmadığını gösterir.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


Yönetici özelliğini alır.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


Uygulamanın adını alır.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


Belge içindeki sayfa sayısının tahmini bir temsilidir.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


Belge içindeki paragraf sayısının tahmini bir temsilidir.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


Belge revizyon numarasını alır.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


Belge küçük resminin görüntüleme modunu gösterir.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


Belgenin konusunu alır.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


Belge şablonunun bilgi adını alır.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Belgenin başlığını alır.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


Toplam düzenleme süresini dakikalar cinsinden alır.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


Belgeyi oluşturan uygulamanın sürüm numarasını temsil eder.

**Remarks**

Biçimi "00.0000" şeklindedir, örneğin: 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


Belge içindeki kelime sayısının tahmini bir temsilidir.

**Returns:**
int
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Adına göre bir özelliğin indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin büyük/küçük harfe duyarsız adı. |

**Returns:**
int - Sıfır tabanlı indeks. Bulunamazsa negatif değer.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Belirtilen ada sahip bir özelliği koleksiyondan kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin büyük/küçük harfe duyarsız adı. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen indeksteki bir özelliği kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Sıfır tabanlı indeks. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Belgenin yazarının adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


Belgedeki bayt sayısının bir tahminini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


Belgenin kategorisini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


Belgedeki karakter sayısının bir tahminini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


Belgedeki karakter (boşluklar dahil) sayısının bir tahminini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Belge yorumlarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


Şirket özelliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


Belgenin içerik durumunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


Belgenin içerik türünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Belgenin oluşturulma tarihini yerel saat diliminde ayarlar.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


Belgenin oluşturulma evrensel zamanını ayarlar.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


Dosyanın sürümünü temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


Köprü tabanı özelliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


Belge anahtar kelimelerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


Belgenin dilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


Belgenin en son yazdırıldığı tarihi yerel saat diliminde ayarlar.

**Remarks**

Belge hiç yazdırılmadıysa, bu özellik DateTime.MinValue döndürecektir.

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


Belgenin en son yazdırıldığı evrensel zamanı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


Son yazarın adını ayarlar.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


En son kaydetmenin zamanını yerel saat diliminde ayarlar.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


En son kaydetmenin evrensel zamanını ayarlar.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


Belge içindeki satır sayısının tahmini bir temsilidir.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


Belgedeki köprülerin güncel olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


Yönetici özelliğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


Uygulamanın adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


Belge içindeki sayfa sayısının tahmini bir temsilidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


Belge içindeki paragraf sayısının tahmini bir temsilidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


Belge revizyon numarasını ayarlar.

**Remarks**

Aspose.Cells, belgeyi değiştirdiğinizde bu özelliği güncellemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


Belge küçük resminin görüntüleme modunu gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


Belgenin konusunu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


Belge şablonunun bilgilendirici adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Belgenin başlığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


Toplam düzenleme süresini dakikalar cinsinden ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


Belgeyi oluşturan uygulamanın sürüm numarasını temsil eder.

**Remarks**

Biçimi "00.0000" şeklindedir, örneğin: 12.0000

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


Belge içindeki kelime sayısının tahmini bir temsilidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

