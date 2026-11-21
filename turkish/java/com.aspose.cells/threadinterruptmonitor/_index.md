---
title: "ThreadInterruptMonitor"
second_title: "Aspose.Cells for Java API Referansı"
description: "Başka bir iş parçacığı başlatarak, kullanıcı tarafından belirtilen uyku süresinden sonra kesintiyi talep etmek için basit bir uygulama."
type: docs
url: /tr/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

Başka bir iş parçacığı başlatarak, kullanıcı tarafından belirtilen uyku süresinden sonra kesintiyi talep etmek için [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) basit bir uygulama.

**Remarks**

Bir izleyici örneği, her süreci sırasıyla izlediğiniz sürece tekrar tekrar kullanılabilir. Çoklu iş parçacıklarında aynı anda birden fazla prosedürü izlemek için kullanılmamalıdır.

**Example**

Aşağıdaki örnek, belirtilen zaman limitiyle yükleme ve kaydetme prosedürünü nasıl izleneceğini gösterir:

```
         ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
         LoadOptions lopts = new LoadOptions();
         lopts.setInterruptMonitor(monitor);
         monitor.startMonitor(1000); //time limit is 1 second
         Workbook wb = new Workbook("Large.xlsx", lopts);
         //if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
         //otherwise finishes the monitor thread and starts to monitor the save procedure
         monitor.finishMonitor();
         monitor.startMonitor(1500); //time limit is 1.5 seconds
         wb.save("result.xlsx");
         monitor.finishMonitor();
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | Bir kesinti izleyicisi oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | Bir prosedür için izleyiciyi sonlandırır. |
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
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
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
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


Bir prosedür için izleyiciyi sonlandırır.

**Remarks**

İzlenen prosedürden sonra bu yöntemi çağırmak, izleyici iş parçacığını özellikle bir kesinti olmadığında (bu prosedürün süresi belirtilen zaman sınırından daha az olduğunda) daha erken serbest bırakabilir.

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

