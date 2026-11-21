---
title: "FontSettingCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Listeyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/fontsettingcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FontSettingCollection extends CollectionBase
```

Listeyi temsil eder [FontSetting](../../com.aspose.cells/fontsetting).
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [appendText(String text)](#appendText-java.lang.String-) | Metni ekler. |
| [clear()](#clear--) | Tüm ayarları temizle. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [deleteText(int index, int count)](#deleteText-int-int-) | Bazı karakterleri sil. |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [format(int startIndex, int length, Font font, StyleFlag flag)](#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Metni yazı tipi ayarıyla biçimlendir. |
| [get(int index)](#get-int-) | İndeksle [FontSetting](../../com.aspose.cells/fontsetting) alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getHtmlString()](#getHtmlString--) | Bu şekilde veri ve bazı biçimlendirmeler içeren html dizesini alır. |
| [getParagraphEnumerator()](#getParagraphEnumerator--) | Paragrafların enumerator'ünü alır. |
| [getText()](#getText--) | Şeklin metnini alır. |
| [getTextAlignment()](#getTextAlignment--) | Metin gövdesinin hizalama ayarını temsil eder. |
| [getTextParagraphs()](#getTextParagraphs--) | Tüm paragrafları alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | İndeksi konuma ekle. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [replace(int index, int count, String text)](#replace-int-int-java.lang.String-) | Metni değiştir. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Metni değiştir. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Bu şekilde veri ve bazı biçimlendirmeler içeren html dizesini ayarlar. |
| [setText(String value)](#setText-java.lang.String-) | Şeklin metnini ayarlar. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Önceden ayarlanmış WordArt stilini ayarlar. |
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
### appendText(String text) {#appendText-java.lang.String-}
```
public void appendText(String text)
```


Metni ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Metin. |

### clear() {#clear--}
```
public void clear()
```


Tüm ayarları temizle.

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
### deleteText(int index, int count) {#deleteText-int-int-}
```
public void deleteText(int index, int count)
```


Bazı karakterleri sil.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Başlangıç indeksi. |
| sayı | int | Karakterlerin sayısı. |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### format(int startIndex, int length, Font font, StyleFlag flag) {#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void format(int startIndex, int length, Font font, StyleFlag flag)
```


Metni yazı tipi ayarıyla biçimlendir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Başlangıç indeksi. |
| length | int | Uzunluk. |
| font | [Font](../../com.aspose.cells/font) | Yazı tipi. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Yazı tipinin bayrakları. |

### get(int index) {#get-int-}
```
public FontSetting get(int index)
```


İndeksle [FontSetting](../../com.aspose.cells/fontsetting) alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - 
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
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Bu şekilde veri ve bazı biçimlendirmeler içeren html dizesini alır.

**Returns:**
java.lang.String
### getParagraphEnumerator() {#getParagraphEnumerator--}
```
public Iterator getParagraphEnumerator()
```


Paragrafların enumerator'ünü alır.

**Returns:**
java.util.Iterator -
### getText() {#getText--}
```
public String getText()
```


Şeklin metnini alır.

**Returns:**
java.lang.String
### getTextAlignment() {#getTextAlignment--}
```
public ShapeTextAlignment getTextAlignment()
```


Metin gövdesinin hizalama ayarını temsil eder.

**Returns:**
[ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)
### getTextParagraphs() {#getTextParagraphs--}
```
public TextParagraphCollection getTextParagraphs()
```


Tüm paragrafları alır.

**Returns:**
[TextParagraphCollection](../../com.aspose.cells/textparagraphcollection)
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
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
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


İndeksi konuma ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Başlangıç indeksi. |
| metin | java.lang.String | Metin. |

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


Belirtilen dizindeki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak öğenin sıfır tabanlı dizini. |

### replace(int index, int count, String text) {#replace-int-int-java.lang.String-}
```
public void replace(int index, int count, String text)
```


Metni değiştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Başlangıç indeksi. |
| sayı | int | Karakterlerin sayısı. |
| metin | java.lang.String | Metin. |

### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public void replace(String oldValue, String newValue)
```


Metni değiştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldValue | java.lang.String | Eski metin. |
| newValue | java.lang.String | Yeni metin. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Bu şekilde veri ve bazı biçimlendirmeler içeren html dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Şeklin metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Önceden ayarlanmış WordArt stilini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Önceden ayarlanmış WordArt stili. |

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

