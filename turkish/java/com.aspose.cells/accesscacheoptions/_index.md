---
title: "AccessCacheOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Veri erişimi için önbellekleme seçenekleri."
type: docs
url: /tr/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Veri erişimi için önbellekleme seçenekleri. Birden fazla seçenek "\|" operatörü kullanılarak birleştirilebilir.

**Remarks**

Bazı özellikler için, büyük veri kümesine erişmek arama, hesaplama gibi çok sayıda tekrarlayan ve karmaşık işlemler gerektirir ve bu işlemler ekstra zaman alır. Yaygın durumlarda, tüm bağımlı veriler erişim sırasında değişmez, bu yüzden bazı önbellekler oluşturulup erişim performansını artırmak için kullanılabilir. Bu amaçla, kullanıcıların hangi veri erişiminin olası önbellekleme mekanizmasıyla optimize edilmesi gerektiğini belirtebilmeleri için bu API'yi sağlıyoruz.

Lütfen unutmayın, farklı seçenekler için farklı veri setlerinin "read-only" olması gerekebilir. Veri erişim performansı birçok faktöre bağlıdır; önbellekleme mekanizmasının kullanılması performansın artacağını garanti etmez. Bazı durumlarda, örneğin erişilecek veri seti küçükse, önbellek kullanmak ekstra zaman gerektirdiği için daha fazla zaman alabilir.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [ALL](#ALL) | Çalışma kitabındaki tüm veri erişim türleri için mümkün olan tüm iyileştirmeleri uygula. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Formüllerin hesaplanması için mümkün olan iyileştirmeyi uygula. |
| [CELLS_DATA](#CELLS-DATA) | Hücre değerlerinin alınması için mümkün olan iyileştirmeyi uygula. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Hücrelerin görüntüyle ilgili sonuçlarının alınması için mümkün olan iyileştirmeyi uygula([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), vb.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Koşullu biçimlendirmelerin biçimleme sonucunun alınması için mümkün olan iyileştirmeyi uygula. |
| [GET_FORMULA](#GET-FORMULA) | Formüllerin alınması için mümkün olan iyileştirmeyi uygula. |
| [NONE](#NONE) | Herhangi bir veri erişimi için önbellek yok. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Nesnenin (örneğin Shape) konum ve boyutunun alınması için mümkün olan iyileştirmeyi uygula. |
| [SET_FORMULA](#SET-FORMULA) | Formüllerin ayarlanması için mümkün olan iyileştirmeyi uygula. |
| [VALIDATION](#VALIDATION) | Doğrulama sonucunun alınması için mümkün olan iyileştirmeyi uygula. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Çalışma kitabındaki tüm veri erişim türleri için mümkün olan tüm iyileştirmeleri uygula. Optimize edilmiş erişim sırasında tüm ayarlar ve veriler değiştirilmemelidir.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Formüllerin hesaplanması için mümkün olan iyileştirmeyi uygula. Optimize edilmiş erişim sırasında hücre verileri değişmemeli, yeni nesneler (Cell, Row vb.) de oluşturulmamalıdır (örneğin [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-) ile).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Hücre değerlerinin alınması için mümkün olan iyileştirmeyi uygula. Optimize edilmiş erişim sırasında hücre verileri (Cell ve Row'un veri ve ayarları) değişmemeli, yeni Cell/Row nesneleri de oluşturulmamalıdır (örneğin [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-) ile).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Hücrelerin görüntüyle ilgili sonuçlarının alınması için mümkün olan iyileştirmeyi uygula([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), vb.). Optimize edilmiş erişim sırasında hücre verileri ve stil ile ilgili nesneler (Cell/Row/Column stilleri, sütun genişliği vb.) değiştirilmemelidir.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Koşullu biçimlendirmelerin biçimlendirme sonucunu alırken olası optimizasyonu uygulayın. Koşullu biçimlendirmelerin sonucunu etkileyebilecek tüm veri ve ayarlar (koşullu biçimlendirme ayarları, bağımlı hücre değerleri vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Formülleri alırken olası optimizasyonu uygulayın. Formül ifadesini etkileyebilecek tüm veri ve ayarlar (Çalışma sayfasının adı, Adın metni, tablonun sütunu vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.

### NONE {#NONE}
```
public static final int NONE
```


Herhangi bir veri erişimi için önbellek yok.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Nesnenin (örneğin Şekil) konum ve boyutunu alırken olası optimizasyonu uygulayın. Satır yüksekliği ve sütun genişliği ayarları optimize edilmiş erişim sırasında değiştirilmemelidir.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Formülleri ayarlarken olası optimizasyonu uygulayın. Formül ifadesini etkileyebilecek tüm veri ve ayarlar (Çalışma sayfasının adı, Adın metni, tablonun sütunu vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Doğrulama sonucunu alırken olası optimizasyonu uygulayın. Doğrulama sonucunu etkileyebilecek tüm veri ve ayarlar (doğrulama ayarları, bağımlı hücre değerleri vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

