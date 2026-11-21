---
title: "DateTime"
second_title: "Aspose.Cells for Java API Referansı"
description: "Genellikle tarih ve günün saat olarak ifade edildiği bir zaman anını temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

Genellikle tarih ve saat olarak ifade edilen bir zaman anını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | DateTime nesnesinin yeni bir örneğini belirtilen yıl, ay ve gün ile başlatır. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Belirtilen yıl, ay, gün, saat, dakika ve saniyeye göre DateTime nesnesinin yeni bir örneğini başlatır. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Belirtilen yıl, ay, gün, saat, dakika, saniye ve milisaniyeye göre DateTime nesnesinin yeni bir örneğini başlatır. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Belirtilen Date nesnesine göre DateTime nesnesinin yeni bir örneğini başlatır. |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Belirtilen Calendar nesnesine göre DateTime nesnesinin yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Bu örneğin değerine belirtilen gün sayısını ekler. |
| [addHours(double value)](#addHours-double-) | Bu örneğin değerine belirtilen saat sayısını ekler. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Bu örneğin değerine belirtilen milisaniye sayısını ekler. |
| [addMinutes(double value)](#addMinutes-double-) | Bu örneğin değerine belirtilen dakika sayısını ekler. |
| [addMonths(int months)](#addMonths-int-) | Bu örneğin değerine belirtilen ay sayısını ekler. |
| [addSeconds(double value)](#addSeconds-double-) | Bu örneğin değerine belirtilen saniye sayısını ekler. |
| [addYears(int value)](#addYears-int-) | Bu örneğin değerine belirtilen yıl sayısını ekler. |
| [compareTo(DateTime value)](#compareTo-com.aspose.gridweb.DateTime-) | Bu örneğin değerini belirtilen bir DateTime değerine karşılaştırır ve bu örneğin belirtilen DateTime değerinden daha erken, aynı ya da daha geç olup olmadığını gösteren bir tam sayı döndürür. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Bu örneğin değerini belirtilen bir DateTime değerini içeren bir nesneye karşılaştırır ve bu örneğin belirtilen DateTime değerinden daha erken, aynı ya da daha geç olup olmadığını gösteren bir tam sayı döndürür. |
| [equals(Object value)](#equals-java.lang.Object-) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Bu örnek tarafından temsil edilen ayın gününü alır. |
| [getDayOfWeek()](#getDayOfWeek--) | Bu örnek tarafından temsil edilen haftanın gününü alır. |
| [getDayOfYear()](#getDayOfYear--) | Bu örnek tarafından temsil edilen yılın gününü alır. |
| [getHour()](#getHour--) | Bu örnek tarafından temsil edilen tarihin saat bileşenini alır. |
| [getMillisecond()](#getMillisecond--) | Bu örnek tarafından temsil edilen tarihin milisaniye bileşenini alır. |
| [getMinute()](#getMinute--) | Bu örnek tarafından temsil edilen tarihin dakika bileşenini alır. |
| [getMonth()](#getMonth--) | Bu örnek tarafından temsil edilen tarihin ay bileşenini alır. |
| [getNow()](#getNow--) | Bu bilgisayarda geçerli tarih ve saate ayarlanmış, yerel zaman olarak ifade edilen bir DateTime nesnesini alır. |
| [getSecond()](#getSecond--) | Bu örnek tarafından temsil edilen tarihin saniye bileşenini alır. |
| [getYear()](#getYear--) | Bu örnek tarafından temsil edilen tarihin yıl bileşenini alır. |
| [hashCode()](#hashCode--) | Bu örnek için karma kodunu döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Geçerli DateTime nesnesinin değerini Calendar nesnesine dönüştürür. |
| [toDate()](#toDate--) | Geçerli DateTime nesnesinin değerini Date nesnesine dönüştürür. |
| [toLocalTime()](#toLocalTime--) | Geçerli DateTime nesnesinin değerini yerel saate dönüştürür. |
| [toString()](#toString--) | Geçerli DateTime nesnesinin değerini eşdeğer dize temsiline dönüştürür. |
| [toUniversalTime()](#toUniversalTime--) | Geçerli DateTime nesnesinin değerini Koordinatlı Evrensel Zaman (UTC)'a dönüştürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


DateTime nesnesinin yeni bir örneğini belirtilen yıl, ay ve gün ile başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yıl | int | Yıl (1 ile 9999 arasında). |
| ay | int | Ay (1 ile 12 arasında). |
| gün | int | Gün (1 ile ay içindeki gün sayısı arasında). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


Belirtilen yıl, ay, gün, saat, dakika ve saniyeye göre DateTime nesnesinin yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yıl | int | Yıl (1 ile 9999 arasında). |
| ay | int | Ay (1 ile 12 arasında). |
| gün | int | Gün (1 ile ay içindeki gün sayısı arasında). |
| saat | int | Saatler (0 ile 23 arasında). |
| dakika | int | Dakikalar (0 ile 59 arasında). |
| saniye | int | Saniyeler (0 ile 59 arasında). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


Belirtilen yıl, ay, gün, saat, dakika, saniye ve milisaniyeye göre DateTime nesnesinin yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yıl | int | Yıl (1 ile 9999 arasında). |
| ay | int | Ay (1 ile 12 arasında). |
| gün | int | Gün (1 ile ay içindeki gün sayısı arasında). |
| saat | int | Saatler (0 ile 23 arasında). |
| dakika | int | Dakikalar (0 ile 59 arasında). |
| saniye | int | Saniyeler (0 ile 59 arasında). |
| milisaniye | int | Milisaniyeler (0 ile 999 arasında). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


Belirtilen Date nesnesine göre DateTime nesnesinin yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarih | java.util.Date | Date nesnesi |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


Belirtilen Calendar nesnesine göre DateTime nesnesinin yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cld | java.util.Calendar | Calendar nesnesi |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


Bu örneğin değerine belirtilen gün sayısını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Tam ve kesirli gün sayısı. Değer parametresi negatif ya da pozitif olabilir. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


Bu örneğin değerine belirtilen saat sayısını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Tam ve kesirli saat sayısı. Değer parametresi negatif ya da pozitif olabilir. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


Bu örneğin değerine belirtilen milisaniye sayısını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Tam ve kesirli milisaniye sayısı. Değer parametresi negatif ya da pozitif olabilir. Bu değerin en yakın tam sayıya yuvarlandığını unutmayın. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


Bu örneğin değerine belirtilen dakika sayısını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Tam ve kesirli dakika sayısı. Değer parametresi negatif ya da pozitif olabilir. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


Bu örneğin değerine belirtilen ay sayısını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aylar | int | Ay sayısı. months parametresi negatif ya da pozitif olabilir. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


Bu örneğin değerine belirtilen saniye sayısını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Tam ve kesirli saniyelerden oluşan bir sayı. value parametresi negatif ya da pozitif olabilir. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


Bu örneğin değerine belirtilen yıl sayısını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Yıllardan oluşan bir sayı. value parametresi negatif ya da pozitif olabilir. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.gridweb.DateTime-}
```
public int compareTo(DateTime value)
```


Bu örneğin değerini belirtilen bir DateTime değerine karşılaştırır ve bu örneğin belirtilen DateTime değerinden daha erken, aynı ya da daha geç olup olmadığını gösteren bir tam sayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.gridweb/datetime) | Karşılaştırma için bir DateTime nesnesi. |

**Returns:**
int - Bu örnek ile value parametresi arasındaki göreli değerleri gösteren işaretli bir sayı. Değer Açıklama Sıfırdan küçük Bu örnek value'dan daha önce. Sıfır Bu örnek value ile aynı. Sıfırdan büyük Bu örnek value'dan daha sonra.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


Bu örneğin değerini belirtilen bir DateTime değerini içeren bir nesneye karşılaştırır ve bu örneğin belirtilen DateTime değerinden daha erken, aynı ya da daha geç olup olmadığını gösteren bir tam sayı döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | Karşılaştırma için kutulanmış bir DateTime nesnesi veya null. |

**Returns:**
int - Bu örnek ile value arasındaki göreli değerleri gösteren işaretli bir sayı. Değer Açıklama Sıfırdan küçük Bu örnek value'dan daha önce. Sıfır Bu örnek value ile aynı. Sıfırdan büyük Bu örnek value'dan daha sonra, veya value null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | Bu örnek ile karşılaştırmak için bir nesne. |

**Returns:**
boolean - value bir DateTime örneği ise ve bu örnek değerine eşitse true; aksi takdirde false.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDay() {#getDay--}
```
public int getDay()
```


Bu örnek tarafından temsil edilen ayın gününü alır.

**Returns:**
int - Gün bileşeni, 1 ile 31 arasında bir değer olarak ifade edilir.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


Bu örnek tarafından temsil edilen haftanın gününü alır.

**Returns:**
int - Bu DateTime değerinin haftanın günü.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


Bu örnek tarafından temsil edilen yılın gününü alır.

**Returns:**
int - Yılın günü, 1 ile 366 arasında bir değer olarak ifade edilir.
### getHour() {#getHour--}
```
public int getHour()
```


Bu örnek tarafından temsil edilen tarihin saat bileşenini alır.

**Returns:**
int - Saat bileşeni, 0 ile 23 arasında bir değer olarak ifade edilir.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


Bu örnek tarafından temsil edilen tarihin milisaniye bileşenini alır.

**Returns:**
int - Milisaniye bileşeni, 0 ile 999 arasında bir değer olarak ifade edilir.
### getMinute() {#getMinute--}
```
public int getMinute()
```


Bu örnek tarafından temsil edilen tarihin dakika bileşenini alır.

**Returns:**
int - Dakika bileşeni, 0 ile 59 arasında bir değer olarak ifade edilir.
### getMonth() {#getMonth--}
```
public int getMonth()
```


Bu örnek tarafından temsil edilen tarihin ay bileşenini alır.

**Returns:**
int - Ay bileşeni, 1 ile 12 arasında bir değer olarak ifade edilir.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


Bu bilgisayarda geçerli tarih ve saate ayarlanmış, yerel zaman olarak ifade edilen bir DateTime nesnesini alır.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


Bu örnek tarafından temsil edilen tarihin saniye bileşenini alır.

**Returns:**
int - Saniyeler, 0 ile 59 arasında.
### getYear() {#getYear--}
```
public int getYear()
```


Bu örnek tarafından temsil edilen tarihin yıl bileşenini alır.

**Returns:**
int - Yıl, 1 ile 9999 arasında.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Bu örnek için karma kodunu döndürür.

**Returns:**
int - 32-bit işaretli bir tamsayı hash kodu.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toCalendar() {#toCalendar--}
```
public Calendar toCalendar()
```


Geçerli DateTime nesnesinin değerini Calendar nesnesine dönüştürür.

**Returns:**
java.util.Calendar - Calendar nesnesi
### toDate() {#toDate--}
```
public Date toDate()
```


Geçerli DateTime nesnesinin değerini Date nesnesine dönüştürür.

**Returns:**
java.util.Date - Date nesnesi
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


Geçerli DateTime nesnesinin değerini yerel saate dönüştürür.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


Geçerli DateTime nesnesinin değerini eşdeğer dize temsiline dönüştürür.

**Returns:**
java.lang.String - Mevcut DateTime nesnesinin değerinin string temsili.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


Geçerli DateTime nesnesinin değerini Koordinatlı Evrensel Zaman (UTC)'a dönüştürür.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of UTC
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

