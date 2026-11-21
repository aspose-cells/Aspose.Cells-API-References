---
title: "AbstractInterruptMonitor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tüm zaman alıcı işlemlerde kesinti isteklerini izlemek için monitör."
type: docs
url: /tr/java/com.aspose.cells/abstractinterruptmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractInterruptMonitor
```

Tüm zaman alıcı işlemlerde kesinti isteklerini izlemek için monitör.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractInterruptMonitor()](#AbstractInterruptMonitor--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | İşlem kesildiğinde, prosedürü sessizce sonlandırıp sonlandırmayacağını veya bir İstisna atıp atmayacağını belirtir. |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Kesintinin mevcut işlem için istenip istenmediğini gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractInterruptMonitor() {#AbstractInterruptMonitor--}
```
public AbstractInterruptMonitor()
```


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
### getTerminateWithoutException() {#getTerminateWithoutException--}
```
public boolean getTerminateWithoutException()
```


İşlem kesintiye uğradığında, işlemi sessizce sonlandırıp sonlandırmayacağını veya bir Exception fırlatıp fırlatmayacağını belirler. Varsayılan değer false'tur, yani [isInterruptionRequested()](../../com.aspose.cells/abstractinterruptmonitor\#isInterruptionRequested--) true olduğunda, [CellsException](../../com.aspose.cells/cellsexception) kodu [ExceptionType.INTERRUPTED](../../com.aspose.cells/exceptiontype\#INTERRUPTED) olan bir istisna fırlatılacaktır.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isInterruptionRequested() {#isInterruptionRequested--}
```
public abstract boolean isInterruptionRequested()
```


Mevcut işlem için kesintinin istenip istenmediğini gösterir. True ise mevcut işlem kesintiye uğrayacaktır. Uygulama burada hızlı ve verimli bir kontrol yapmalıdır, aksi takdirde prosedür için başka bir darboğaz haline gelebilir.

**Returns:**
boolean
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

