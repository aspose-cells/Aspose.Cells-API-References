---
title: "InterruptMonitor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kesintiyle ilgili tüm operatörleri temsil eder."
type: docs
url: /tr/java/com.aspose.cells/interruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class InterruptMonitor extends AbstractInterruptMonitor
```

Kesintiyle ilgili tüm operatörleri temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [InterruptMonitor()](#InterruptMonitor--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | İşlem kesildiğinde, prosedürü sessizce sonlandırıp sonlandırmayacağını veya bir İstisna atıp atmayacağını belirtir. |
| [hashCode()](#hashCode--) |  |
| [interrupt()](#interrupt--) | Mevcut operatörü kes. |
| [isInterruptionRequested()](#isInterruptionRequested--) | Monitörü kesinti talep ediyor olarak işaretle |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### InterruptMonitor() {#InterruptMonitor--}
```
public InterruptMonitor()
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
### interrupt() {#interrupt--}
```
public void interrupt()
```


Mevcut operatörü kes.

### isInterruptionRequested() {#isInterruptionRequested--}
```
public boolean isInterruptionRequested()
```


Monitörü kesinti talep ediyor olarak işaretle

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

