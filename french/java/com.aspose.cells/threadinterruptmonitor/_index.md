---
title: "ThreadInterruptMonitor"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Implémentation simple de  en démarrant un autre thread pour demander l'interruption après une pause de la limite spécifiée par l'utilisateur."
type: docs
url: /fr/java/com.aspose.cells/threadinterruptmonitor/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
```
public class ThreadInterruptMonitor extends AbstractInterruptMonitor
```

Implémentation simple de [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) en démarrant un autre thread pour demander l'interruption après une pause de la limite spécifiée par l'utilisateur.

**Remarks**

Une instance de moniteur peut être utilisée de manière répétée, tant que vous surveillez chaque processus séquentiellement. Elle ne doit pas être utilisée pour surveiller plusieurs procédures simultanément dans des threads multiples.

**Example**

L'exemple suivant montre comment surveiller la procédure de chargement et d'enregistrement avec une limite de temps spécifiée :

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
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ThreadInterruptMonitor(boolean terminateWithoutException)](#ThreadInterruptMonitor-boolean-) | Construit un moniteur d'interruption. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finishMonitor()](#finishMonitor--) | Termine le moniteur pour une procédure. |
| [getClass()](#getClass--) |  |
| [getTerminateWithoutException()](#getTerminateWithoutException--) | Voir [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). |
| [hashCode()](#hashCode--) |  |
| [isInterruptionRequested()](#isInterruptionRequested--) | Cette implémentation vérifie simplement si le temps écoulé (du moment où ce moniteur a été démarré jusqu'à maintenant) est supérieur à la limite spécifiée par l'utilisateur. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [startMonitor(int msLimit)](#startMonitor-int-) | Démarre le moniteur avec la limite de temps spécifiée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThreadInterruptMonitor(boolean terminateWithoutException) {#ThreadInterruptMonitor-boolean-}
```
public ThreadInterruptMonitor(boolean terminateWithoutException)
```


Construit un moniteur d'interruption.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--) |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### finishMonitor() {#finishMonitor--}
```
public void finishMonitor()
```


Termine le moniteur pour une procédure.

**Remarks**

Appeler cette méthode après la procédure surveillée peut libérer le thread du moniteur plus tôt, surtout lorsqu'il n'y a aucune interruption pour celle‑ci (le temps d'exécution de cette procédure est inférieur à la limite de temps spécifiée).

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


Voir [AbstractInterruptMonitor.getTerminateWithoutException()](../../com.aspose.cells/abstractinterruptmonitor\#getTerminateWithoutException--). Cette propriété est spécifiée par l'utilisateur lors de la construction de cette instance de moniteur.

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


Cette implémentation vérifie simplement si le temps écoulé (du moment où ce moniteur a été démarré jusqu'à maintenant) est supérieur à la limite spécifiée par l'utilisateur.

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


Démarre le moniteur avec la limite de temps spécifiée. Le temps de départ pour calculer le coût en temps est exactement le moment où cette méthode est appelée, ainsi la procédure à surveiller doit être démarrée immédiatement après cet appel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| msLimit | int | limite de temps (ms) pour demander l'interruption. |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

