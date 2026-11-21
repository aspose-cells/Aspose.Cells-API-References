---
title: "PictureCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/picturecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PictureCollection extends CollectionBase
```

Bir [Picture](../../com.aspose.cells/picture) nesnesi koleksiyonunu kapsüller.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get PictureCollection
         PictureCollection pictures = workbook.getWorksheets().get(0).getPictures();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#add-int-int-int-int-java.io.InputStream-) | Koleksiyona bir resim ekler. |
| [add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)](#add-int-int-int-int-java.lang.String-) | Koleksiyona bir resim ekler. |
| [add(int topRow, int leftColumn, InputStream stream)](#add-int-int-java.io.InputStream-) | Koleksiyona bir resim ekler. |
| [add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#add-int-int-java.io.InputStream-int-int-) | Koleksiyona bir resim ekler. |
| [add(int topRow, int leftColumn, String fileName)](#add-int-int-java.lang.String-) | Koleksiyona bir resim ekler. |
| [add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)](#add-int-int-java.lang.String-int-int-) | Koleksiyona bir resim ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [camera(int row, int column, String range)](#camera-int-int-java.lang.String-) | Aralığın fotoğrafını çeker. |
| [clear()](#clear--) | Tüm resimleri temizle. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [Picture](../../com.aspose.cells/picture) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirli indeksteki şekilleri kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#add-int-int-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Koleksiyona bir resim ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| bottomRow | int | Alt sağ satır indeksi |
| rightColumn | int | Alt sağ sütun indeksi |
| stream | java.io.InputStream | Görüntü verilerini içeren akış nesnesi. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) nesne indeksi.
### add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName) {#add-int-int-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, int bottomRow, int rightColumn, String fileName)
```


Koleksiyona bir resim ekler.

**Example**

```
         //add a picture
         pictures.add(1, 1, 5, 5, "image.jpg");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| bottomRow | int | Alt sağ satır indeksi |
| rightColumn | int | Alt sağ sütun indeksi |
| fileName | java.lang.String | Resim dosya adı. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) nesne indeksi.
### add(int topRow, int leftColumn, InputStream stream) {#add-int-int-java.io.InputStream-}
```
public int add(int topRow, int leftColumn, InputStream stream)
```


Koleksiyona bir resim ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| stream | java.io.InputStream | Görüntü verilerini içeren akış nesnesi. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) nesne indeksi.
### add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#add-int-int-java.io.InputStream-int-int-}
```
public int add(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Koleksiyona bir resim ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| stream | java.io.InputStream | Görüntü verilerini içeren akış nesnesi. |
| widthScale | int | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | int | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) nesne indeksi.
### add(int topRow, int leftColumn, String fileName) {#add-int-int-java.lang.String-}
```
public int add(int topRow, int leftColumn, String fileName)
```


Koleksiyona bir resim ekler.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| fileName | java.lang.String | Resim dosya adı. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) nesne indeksi.
### add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale) {#add-int-int-java.lang.String-int-int-}
```
public int add(int topRow, int leftColumn, String fileName, int widthScale, int heightScale)
```


Koleksiyona bir resim ekler.

**Example**

```
         //add a picture
         pictures.add(1, 1, "image.jpg", 50, 50);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| fileName | java.lang.String | Resim dosya adı. |
| widthScale | int | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | int | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

**Returns:**
int - [Picture](../../com.aspose.cells/picture) nesne indeksi.
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
### camera(int row, int column, String range) {#camera-int-int-java.lang.String-}
```
public int camera(int row, int column, String range)
```


Aralığın fotoğrafını çeker.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Bu resmin satır indeksi. |
| sütun | int | Bu resmin sütun indeksi. |
| aralık | java.lang.String | Fotoğraf çekilmesi gereken alan |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Tüm resimleri temizle.

**Example**

```
         //clear
         pictures.clear();
```

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
public Picture get(int index)
```


Belirtilen indeksteki [Picture](../../com.aspose.cells/picture) öğesini alır.

**Example**

```
         //get picture collection
         //PictureCollection pictures = workbook.Worksheets[0].Pictures;
         //add a picture
         int index = pictures.add(1, 1, "image.png");
         //get the picture
         Picture pic = pictures.get(index);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - The element at the specified index.
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirli indeksteki şekilleri kaldır.

**Example**

```
         //add a picture
         int index2 = pictures.add(1, 1, "image.png");
         //delete
         pictures.removeAt(index2);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

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

