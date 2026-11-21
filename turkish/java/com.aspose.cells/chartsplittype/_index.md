---
title: "ChartSplitType"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pasta içinde pasta grafiği ya da pasta içinde çubuk grafiğinin iki bölümünün nasıl bölündüğünü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/chartsplittype/
---

**Inheritance:**
java.lang.Object
```
public final class ChartSplitType
```

Pasta içinde pasta grafiği ya da pasta içinde çubuk grafiğinin iki bölümünün nasıl bölündüğünü temsil eder.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [AUTO](#AUTO) | Bu grafik türü için varsayılan mekanizma kullanılarak bölünecek veri noktalarını temsil eder. |
| [CUSTOM](#CUSTOM) | Veri noktalarının, Özel Bölme değerlerine göre pasta ve ikinci grafik arasında bölüneceğini temsil eder. |
| [PERCENT_VALUE](#PERCENT-VALUE) | Veri noktalarının, Bölme Pozisyonu yüzdesinden daha düşük yüzdeye sahip noktaları ikinci grafiğe yerleştirerek pasta ve ikinci grafik arasında bölüneceğini temsil eder. |
| [POSITION](#POSITION) | Veri noktalarını temsil eder. |
| [VALUE](#VALUE) | Veri noktalarının, Bölme Pozisyonundan daha düşük değere sahip veri noktalarını ikinci grafiğe yerleştirerek pasta ve ikinci grafik arasında bölüneceğini temsil eder. |
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
### AUTO {#AUTO}
```
public static final int AUTO
```


Bu grafik türü için varsayılan mekanizma kullanılarak bölünecek veri noktalarını temsil eder.

**Remarks**

NOTE: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Series.IsAutoSplit özelliğini kullanın. Bu özellik, Eylül 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Veri noktalarının, Özel Bölme değerlerine göre pasta ve ikinci grafik arasında bölüneceğini temsil eder.

### PERCENT_VALUE {#PERCENT-VALUE}
```
public static final int PERCENT_VALUE
```


Veri noktalarının, Bölme Pozisyonu yüzdesinden daha düşük yüzdeye sahip noktaları ikinci grafiğe yerleştirerek pasta ve ikinci grafik arasında bölüneceğini temsil eder.

### POSITION {#POSITION}
```
public static final int POSITION
```


Veri noktalarını temsil eder. Veri noktalarının, son bölme konumunu ikinci grafiğe yerleştirerek pasta ve ikinci grafik arasında bölünecektir.

### VALUE {#VALUE}
```
public static final int VALUE
```


Veri noktalarının, Bölme Pozisyonundan daha düşük değere sahip veri noktalarını ikinci grafiğe yerleştirerek pasta ve ikinci grafik arasında bölüneceğini temsil eder.

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

