---
title: "CalculationData"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir fonksiyonun (örneğin fonksiyon adı parametreleri ... vb.) hesaplanması sırasında gereken verileri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

Bir fonksiyonun hesaplanması sırasında gerekli verileri temsil eder; örneğin fonksiyon adı, parametreler, vb.

**Remarks**

Bu sınıf tarafından sağlanan tüm nesneler yalnızca "okuma" amacıyla kullanılabilir. Kullanıcı, formül hesaplama sürecinde Workbook'taki herhangi bir veriyi değiştirmemelidir, aksi takdirde beklenmeyen sonuçlar veya istisna oluşabilir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Bu fonksiyon için hesaplanan değeri alır. |
| [getCell()](#getCell--) | Fonksiyonun bulunduğu Cell nesnesini alır. |
| [getCellColumn()](#getCellColumn--) | Fonksiyonun bulunduğu hücrenin sütun indeksini alır. |
| [getCellRow()](#getCellRow--) | Fonksiyonun bulunduğu hücrenin satır indeksini alır. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Hesaplanacak fonksiyon adını alır. |
| [getParamCount()](#getParamCount--) | Parametre sayısını alır |
| [getParamText(int index)](#getParamText-int-) | Verilen indeksdeki parametrenin literal metnini alır. |
| [getParamValue(int index)](#getParamValue-int-) | Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | Verilen indeksdeki parametrenin değer(ler)ini alır. |
| [getWorkbook()](#getWorkbook--) | Fonksiyonun bulunduğu Workbook nesnesini alır. |
| [getWorksheet()](#getWorksheet--) | Fonksiyonun bulunduğu Worksheet nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Bu fonksiyon için hesaplanmış değeri ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Bu fonksiyon için hesaplanan değeri alır.

**Remarks**

Kullanıcı, motorun desteklediği fonksiyonlar için bu özelliği kendi özel hesaplama motorunda ayarlamalıdır; ayarlanan değer daha sonra bu özellik alındığında döndürülür. Ayarlanan değer, olası tiplerden biri olan [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) ya da bu tür değerlerin dizisi, ya da bir Range, Name, ReferredArea olabilir. Bu özelliğe değer atanmadan önce alınması, fonksiyonun Aspose.Cells'in varsayılan hesaplama motoru tarafından hesaplanmasına ve ardından hesaplanmış değerin döndürülmesine (genellikle kullanıcı tanımlı fonksiyonlar için \#NAME? olmalıdır) neden olur.

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


Fonksiyonun bulunduğu Cell nesnesini alır.

**Remarks**

Bir formül hücreye ayarlanmadan, örneğin [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-) ile hesaplandığında, formül A1 hücresine ayarlanmış gibi hesaplanır, bu yüzden hem [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) hem de [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) 0 olur. Ancak, çalışma sayfasındaki A1 hücresi henüz oluşturulmamış olabilir. Bu tür durumlar için bu özellik null olacaktır.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Fonksiyonun bulunduğu hücrenin sütun indeksini alır.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Fonksiyonun bulunduğu hücrenin satır indeksini alır.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Hesaplanacak fonksiyon adını alır.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Parametre sayısını alır

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Verilen indeksdeki parametrenin literal metnini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | parametrenin indeksi (0 tabanlı) |

**Returns:**
java.lang.String - parametrenin literal metni.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır.

**Remarks**

Tek bir parametre için:

Eğer düz bir değer ise, düz değeri kendisini döndürür;

Eğer bir referans ise, ReferredArea nesnesini döndürür;

Eğer birden fazla değere sahip veri kümesine referans veriyorsa, nesneler dizisini döndürür;

Eğer hesaplanması gereken bir ifade ise, mevcut hücre temeline göre değer modunda hesaplanır ve genellikle tek bir değer döndürülür. Örneğin, D2 formülünün bir parametresi A:A+B:B ise, A2+B2 hesaplanıp döndürülür. Ancak, bu parametre dizi modu olarak belirtilmişse (by  or ), A1+B1, A2+B2, ... öğelerinden oluşan bir dizi (object[][]) döndürülür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Parametrenin indeksi (0 tabanlı) |

**Returns:**
java.lang.Object - Parametrenin hesaplanmış değeri.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


Verilen indeksdeki parametrenin değer(ler)ini alır. Parametre, hesaplanması gereken bir ifade ise, dizi modunda hesaplanır.

**Remarks**

Calculable bir ifade için, A:A+B:B örneğini alalım: Değer modunda, mevcut hücre temeline göre tek bir değere hesaplanır. Ancak dizi modunda, A1+B1, A2+B2, A3+B3, ... tüm değerleri hesaplanır ve döndürülen dizi oluşturmak için kullanılır. Bu tür durumlar için satır/sütun sayısı sınırını (örneğin [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) ve [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--) değerlerine göre) belirtmek daha iyidir; aksi takdirde döndürülen büyük dizi, gereksiz verilerle bellek maliyetini artırabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Parametrenin indeksi (0 tabanlı) |
| maxRowCount | int | Döndürülen dizi için satır sayısı sınırı. Eğer pozitif değilse veya gerçek satır sayısından büyükse, gerçek satır sayısı kullanılır. |
| maxColumnCount | int | Döndürülen dizi için sütun sayısı sınırı. Eğer pozitif değilse veya gerçek satır sayısından büyükse, gerçek sütun sayısı kullanılır. |

**Returns:**
java.lang.Object[][] - Belirtilen parametre tarafından temsil edilen tüm öğeleri içeren bir dizi.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Fonksiyonun bulunduğu Workbook nesnesini alır.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Fonksiyonun bulunduğu Worksheet nesnesini alır.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Bu fonksiyon için hesaplanmış değeri ayarlar.

**Remarks**

Kullanıcı, motorun desteklediği fonksiyonlar için bu özelliği kendi özel hesaplama motorunda ayarlamalıdır; ayarlanan değer daha sonra bu özellik alındığında döndürülür. Ayarlanan değer, olası tiplerden biri olan [Cell.getValue()](../../com.aspose.cells/cell\#getValue--) ya da bu tür değerlerin dizisi, ya da bir Range, Name, ReferredArea olabilir. Bu özelliğe değer atanmadan önce alınması, fonksiyonun Aspose.Cells'in varsayılan hesaplama motoru tarafından hesaplanmasına ve ardından hesaplanmış değerin döndürülmesine (genellikle kullanıcı tanımlı fonksiyonlar için \#NAME? olmalıdır) neden olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

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

