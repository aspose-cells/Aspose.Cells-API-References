---
title: "MemorySetting"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre veri modeli için bellek kullanım modları."
type: docs
url: /tr/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

Hücre veri modeli için bellek kullanım modları.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | Bellek performansı tercih edilir ve hücre verilerini tutmak için belleğin yerine dosya kullanılır. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Bellek performansı tercih edilir. |
| [NORMAL](#NORMAL) | Hücre modeli için varsayılan mod. |
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
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```


Bellek performansı tercih edilir ve hücre verilerini tutmak için belleğin yerine dosya kullanılır.

**Remarks**

Bu modda hücre verileri sıkıştırılmış formatta tutulur ve verilerin büyük bir kısmı bellek yerine geçici dosyada tutulur. Bu nedenle [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) modu ile karşılaştırıldığında, bu mod bellek maliyetini daha fazla azaltabilir, ancak hücre verilerine erişim için IO işlemleri daha yüksek zaman maliyeti oluşturur.

Bu seçenek v25.7.0 sürümünden itibaren kullanılabilir.

| Bu modu kullanırken bazı önemli sınırlamalar ve önerilen işlemler: |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Bu mod bir çalışma kitabındaki herhangi bir çalışma sayfası için kullanıldığında, geçici dosyalar gibi tüm kaynakları serbest bırakmak için işin sonunda [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) çağrılmalıdır. |
| Hücrelere rastgele erişim, verilerin rastgele ve tekrar tekrar okunması gerektiği için düşük performans verir (bu nedenle dosyadaki gösterici buna göre değişir ve IO işlemleri tekrar tekrar gerekir). Mümkünse, lütfen veriye her zaman sıralı olarak (satır satır) erişin. |
| Bir satır/hücre verisi değiştirildiğinde, diğer hücrelerin/satırların verileri de etkilenebilir (örneğin değişen veri için yeterli alan ayrılması amacıyla veriler başka yerlere kaydırılabilir). Bu nedenle her veri değişikliği, diğer mevcut nesnelerin (örneğin Satır veya Hücre nesnesi) senkronizasyonunu gerektirir. Daha iyi performans elde etmek için lütfen aynı anda birden fazla Satır/Hücre tutmayın. Onları tek tek işlemek, veri senkronizasyonunu azaltır ve performansın iyileşmesini sağlar. |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


Bellek performansı tercih edilir.

**Remarks**

Bu modda hücre verileri bellek maliyetini azaltmak için sıkıştırılmış formatta tutulur. Öte yandan, sıkıştırılmış veri özellikle hücre verileri güncellenirken veya rastgele erişildiğinde daha yüksek zaman maliyetine neden olabilir.

Bu seçenek v8.0.0 sürümünden itibaren kullanılabilir.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Hücre modeli için varsayılan mod.

**Remarks**

Bu mod tüm sürümler için uygulanır.

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

