---
title: "ThreadInterruptMonitor"
second_title: "Aspose.Cells för Java API-referens"
description: "Enkel implementation av  genom att starta en annan tråd för att kräva avbrott efter att ha sovit i den av användaren angivna gränsen."
type: docs
url: /sv/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

Enkel implementation av [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) genom att starta en annan tråd för att kräva avbrott efter att ha sovit i den av användaren angivna gränsen.

**Remarks**

En monitorinstans kan användas upprepade gånger, så länge du övervakar varje process i sekvens. Den bör inte användas för att övervaka flera procedurer samtidigt i flera trådar.

**Example**

Följande exempel visar hur man övervakar laddnings- och sparproceduren med en specificerad tidsgräns:

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | Skapar en avbrottsövervakare. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | Avslutar monitorn för en procedur. |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Se [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Denna implementation kontrollerar bara om tidskostnaden (från det att övervakaren startades till nu) är större än den användarspecificerade gränsen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | Startar övervakaren med den specificerade tidsgränsen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```


Skapar en avbrottsövervakare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


Avslutar monitorn för en procedur.

**Remarks**

Att anropa den här metoden efter den övervakade proceduren kan frigöra monitortråden tidigare, särskilt när det inte finns något avbrott för den (tidskostnaden för den proceduren är mindre än den angivna tidsgränsen).

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


Se [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). Denna egenskap specificeras av användaren när denna övervakningsinstans konstrueras.

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


Denna implementation kontrollerar bara om tidskostnaden (från det att övervakaren startades till nu) är större än den användarspecificerade gränsen.

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


Startar övervakaren med den specificerade tidsgränsen. Starttiden för att beräkna tidskostnaden är precis när denna metod anropas, så proceduren som ska övervakas bör startas omedelbart efter detta anrop.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| msLimit | int | tidsgräns (ms) för att kräva avbrottet. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

