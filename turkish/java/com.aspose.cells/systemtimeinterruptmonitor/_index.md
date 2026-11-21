---
title: "SystemTimeInterruptMonitor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcı tarafından belirtilen limit ile geçerli sistem saatini kontrol edip karşılaştırarak basit bir uygulama."
type: docs
url: /tr/java/com.aspose.cells/systemtimeinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class SystemTimeInterruptMonitor extends AbstractInterruptMonitor
```

Geçerli sistem saatini kullanıcı tarafından belirtilen limit ile kontrol edip karşılaştırarak [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) için basit bir uygulama.

**Remarks**

Bu uygulama, basit senaryolar için yalnızca basit bir çözümdür. Sistem saatini sık sık alıp kontrol etmesi gerektiğinden, performans üzerinde bir miktar olumsuz etkisi olabilir.

**Example**

Aşağıdaki örnek, belirtilen zaman limitiyle yükleme ve kaydetme prosedürünü nasıl izleneceğini gösterir:

```
         SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
         LoadOptions lopts = new LoadOptions();
         lopts.setInterruptMonitor(monitor);
         monitor.startMonitor(1000); //time limit is 1 second
         Workbook wb = new Workbook("Large.xlsx", lopts);
         //if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
         //otherwise starts to monitor the save procedure
         monitor.startMonitor(1500); //time limit is 1.5 seconds
         wb.save("result.xlsx");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SystemTimeInterruptMonitor(boolean terminateWithoutException)](#SystemTimeInterruptMonitor-boolean-) | Bir kesinti izleyicisi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Bakınız [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Bu uygulama yalnızca zaman maliyetinin (bu izleyicinin başlatıldığı zamandan şu ana kadar) kullanıcı tarafından belirtilen limitten büyük olup olmadığını kontrol eder. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | İzleyiciyi belirtilen zaman limitiyle başlatır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SystemTimeInterruptMonitor(boolean terminateWithoutException) {#SystemTimeInterruptMonitor-boolean-}
```
public SystemTimeInterruptMonitor(boolean terminateWithoutException)
```


Bir kesinti izleyicisi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

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


Bakınız [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). Bu özellik, izleyici örneği oluşturulurken kullanıcı tarafından belirtilir.

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
public boolean isInterruptionRequested()
```


Bu uygulama yalnızca zaman maliyetinin (bu izleyicinin başlatıldığı zamandan şu ana kadar) kullanıcı tarafından belirtilen limitten büyük olup olmadığını kontrol eder.

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




### startMonitor(int msLimit) {#startMonitor-int-}
```
public void startMonitor(int msLimit)
```


Belirtilen zaman sınırıyla izleyiciyi başlatır. Zaman maliyetini hesaplamak için başlangıç zamanı, bu metodun çağrıldığı an olur; bu yüzden izlenmesi gereken prosedür bu çağrının hemen ardından başlatılmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| msLimit | int | Kesintiyi gerektirecek zaman sınırı (ms). |

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

