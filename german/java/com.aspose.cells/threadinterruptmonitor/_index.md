---
title: "ThreadInterruptMonitor"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Einfache Implementierung von  durch Starten eines anderen Threads, um die Unterbrechung nach dem Schlafen der vom Benutzer festgelegten Grenze zu erfordern."
type: docs
url: /de/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

Einfache Implementierung von [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) durch Starten eines anderen Threads, um die Unterbrechung nach dem Schlafen der vom Benutzer festgelegten Grenze zu erfordern.

**Remarks**

Eine Monitorinstanz kann wiederholt verwendet werden, solange Sie jeden Prozess nacheinander überwachen. Sie sollte nicht verwendet werden, um mehrere Verfahren gleichzeitig in mehreren Threads zu überwachen.

**Example**

Das folgende Beispiel zeigt, wie man den Ladevorgang und das Speichern mit einem angegebenen Zeitlimit überwacht:

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
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | Konstruiert einen Unterbrechungsmonitor. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | Beendet den Monitor für ein Verfahren. |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Siehe [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Diese Implementierung prüft lediglich, ob die Zeitkosten (seit dem Start dieses Monitors bis jetzt) größer sind als das vom Benutzer festgelegte Limit. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | Startet den Monitor mit dem angegebenen Zeitlimit. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```


Konstruiert einen Unterbrechungsmonitor.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


Beendet den Monitor für ein Verfahren.

**Remarks**

Der Aufruf dieser Methode nach dem überwachten Verfahren kann den Monitor-Thread früher freigeben, insbesondere wenn keine Unterbrechung dafür erfolgt (die Ausführungszeit dieses Verfahrens ist kürzer als die angegebene Zeitbegrenzung).

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


Siehe [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). Diese Eigenschaft wird vom Benutzer beim Erzeugen dieser Monitorinstanz angegeben.

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


Diese Implementierung prüft lediglich, ob die Zeitkosten (seit dem Start dieses Monitors bis jetzt) größer sind als das vom Benutzer festgelegte Limit.

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


Startet den Monitor mit dem angegebenen Zeitlimit. Der Startzeitpunkt zur Berechnung der Zeitkosten ist genau der Moment, in dem diese Methode aufgerufen wird, sodass das zu überwachende Verfahren unmittelbar nach diesem Aufruf gestartet werden sollte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| msLimit | int | Zeitlimit (ms), um die Unterbrechung zu erzwingen. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

