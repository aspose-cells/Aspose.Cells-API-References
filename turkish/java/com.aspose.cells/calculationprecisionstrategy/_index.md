---
title: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hesaplama hassasiyetini ele alma stratejilerini listeler."
type: docs
url: /tr/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

Hesaplama hassasiyetini ele almak için stratejileri listeler. IEEE 754 kayan nokta aritmetiğinin hassasiyet sorunu nedeniyle, bazı "görünüşte basit" formüller beklenen sonuç olarak hesaplanmayabilir. Örneğin "=-0.45+0.43+0.02" formülü, operantları '+' operatörüyle doğrudan hesaplandığında sonuç sıfır olmaz. Bu tür hassasiyet sorunları için, bazı özel stratejiler beklenen sonucu verebilir.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [DECIMAL](#DECIMAL) | Mümkün olduğunda operand olarak ondalık kullanır. |
| [NONE](#NONE) | Hesaplamada strateji uygulanmadı. |
| [ROUND](#ROUND) | Hesaplama sonucunu anlamlı basamaklara göre yuvarlar. |
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
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Mümkün olduğunda ondalık sayıları operand olarak kullanır. Performans açısından en verimsizidir.

### NONE {#NONE}
```
public static final int NONE
```


Hesaplamada strateji uygulanmaz. Hesaplama yaparken sadece orijinal double değerini operand olarak kullanır ve sonucu doğrudan döndürür. Performans açısından en verimli ve çoğu durumda uygulanabilir.

### ROUND {#ROUND}
```
public static final int ROUND
```


Hesaplama sonucunu anlamlı basamaklara göre yuvarlar.

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

