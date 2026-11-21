---
title: "Ölçülen"
second_title: "Aspose.Cells for Java API Referansı"
description: "Ölçülen anahtarı ayarlamak için yöntemler sağlar."
type: docs
url: /tr/java/com.aspose.cells/metered/
---

**Inheritance:**
java.lang.Object
```
public class Metered
```

Ölçülen anahtarı ayarlamak için yöntemler sağlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Metered()](#Metered--) | Bu sınıfın yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getConsumptionCredit()](#getConsumptionCredit--) | Tüketim kredisini alır |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Tüketim dosya boyutunu alır |
| [getProductName()](#getProductName--) | Ürün adını alır |
| [hashCode()](#hashCode--) |  |
| [isMeteredLicensed()](#isMeteredLicensed--) | Ölçülenin lisanslı olup olmadığını kontrol et |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Ölçülenin genel ve özel anahtarını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Metered() {#Metered--}
```
public Metered()
```


Bu sınıfın yeni bir örneğini başlatır.

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
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Tüketim kredisini alır

**Returns:**
double - tüketim miktarı
### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Tüketim dosya boyutunu alır

**Returns:**
double - tüketim miktarı
### getProductName() {#getProductName--}
```
public String getProductName()
```


Ürün adını alır

**Returns:**
java.lang.String - ürün adı
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMeteredLicensed() {#isMeteredLicensed--}
```
public static boolean isMeteredLicensed()
```


Ölçülenin lisanslı olup olmadığını kontrol et

**Returns:**
boolean - Doğru veya yanlış
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public void setMeteredKey(String publicKey, String privateKey)
```


Ölçülenin genel ve özel anahtarını ayarlar. Ölçülen lisansı satın alırsanız, uygulamayı başlattığınızda bu API çağrılmalıdır, genellikle bu yeterlidir. Ancak, tüketim verilerini yükleme sürekli başarısız olur ve 24 saat aşarsa, lisans değerlendirme durumuna ayarlanır; böyle bir durumu önlemek için lisans durumunu düzenli olarak kontrol etmelisiniz, eğer değerlendirme durumundaysa, bu API'yi tekrar çağırın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| publicKey | java.lang.String | genel anahtar |
| privateKey | java.lang.String | özel anahtar |

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

