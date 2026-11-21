---
title: "RowCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma sayfasındaki bireysel satırları temsil eden nesneleri toplar."
type: docs
url: /tr/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Bir çalışma sayfasındaki bireysel satırları temsil eden [Row](../../com.aspose.cells/row) nesnelerini toplar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [clear()](#clear--) | Tüm satırları ve hücreleri temizle. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Verilen satır indeksine göre bir [Row](../../com.aspose.cells/row) nesnesi alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Bu koleksiyondaki satır sayısını alır. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Listede konuma göre satır nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Bu koleksiyon içinde satırları yineleyen bir enumerator alır |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Bu koleksiyon içinde satırları yineleyen bir enumerator alır |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Bu koleksiyonda belirtilen indeks (konum) konumundaki satır öğesini kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Tüm satırları ve hücreleri temizle.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Verilen satır indeksine göre bir [Row](../../com.aspose.cells/row) nesnesi alır. Verilen satır indeksinin Row nesnesi daha önce mevcut değilse oluşturulur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


Bu koleksiyondaki satır sayısını alır.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Listede konuma göre satır nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Pozisyon. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Bu koleksiyon içinde satırları yineleyen bir enumerator alır

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - Bu koleksiyondaki mevcut tüm satırları dolaşacak satır yineleyicisi.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Bu koleksiyon içinde satırları yineleyen bir enumerator alır

**Remarks**

Eğer satır koleksiyonu, yineleyici ile dolaşım sırasında (yeni Row oluşturulmasına veya mevcut Row'ın kaldırılmasına neden olabilecek işlemlerle) değiştirilirse, dolaşımın son MoveNext() tarafından gezilen konumun hemen sonrasından devam edebilmesi için normal yineleyici yerine eşzamanlı yineleyici kullanılmalıdır. Ancak, hiçbir öğenin atlanmaması veya tekrar tekrar gezilmemesi avantajına ek olarak, eşzamanlı yineleyicinin dezavantajı, normal yineleyiciye kıyasla performansın biraz düşmesidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ters | boolean | satırları ters sırada enumerate edip etmeyeceği |
| eşzamanlı | boolean | dönen yineleyicinin satır koleksiyonundaki değişiklikleri kontrol edip onunla eşzamanlı kalıp kalmayacağı. |

**Returns:**
java.util.Iterator - Bu koleksiyondaki mevcut tüm satırları dolaşacak satır yineleyicisi.
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


Bu koleksiyonda belirtilen indeks (konum) konumundaki satır öğesini kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | bu koleksiyondaki mevcut satır öğesinin sıfır tabanlı indeksi (konumu, [Row.getIndex()](../../com.aspose.cells/row\#getIndex--) değil). |

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

