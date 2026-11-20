---
title: "MemorySetting"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Speichernutzungsmodi für das Zellen‑Datenmodell."
type: docs
url: /de/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

Speichernutzungsmodi für das Zellen‑Datenmodell.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | Speicherleistung ist vorzuziehen und es wird eine Datei anstelle des Speichers verwendet, um die Zellen­daten zu verwalten. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Speicherleistung ist vorzuziehen. |
| [NORMAL](#NORMAL) | Standardmodus für das Zellenmodell. |
## Methoden

| Methode | Beschreibung |
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


Speicherleistung ist vorzuziehen und es wird eine Datei anstelle des Speichers verwendet, um die Zellen­daten zu verwalten.

**Remarks**

In diesem Modus werden die Zellen­daten in kompaktem Format gespeichert und der Großteil der Daten wird in einer temporären Datei anstelle des Speichers gehalten. Beim Vergleich mit dem Modus [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) kann dieser Modus den Speicherverbrauch weiter reduzieren, jedoch verursachen die I/O‑Operationen zum Zugriff auf die Zellen­daten höhere Zeitkosten.

Diese Option ist seit v25.7.0 verfügbar.

| Einige bemerkenswerte Einschränkungen und empfohlene Vorgehensweisen bei Verwendung dieses Modus: |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Wenn dieser Modus für ein beliebiges Arbeitsblatt in einer Arbeitsmappe verwendet wird, sollte am Ende der Arbeit [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) aufgerufen werden, um alle Ressourcen wie die temporären Dateien freizugeben. |
| Zufälliger Zugriff auf Zellen führt zu schlechter Leistung, weil Daten zufällig und wiederholt gelesen werden müssen (so wird der Zeiger in der Datei entsprechend verschoben und I/O‑Operationen werden wiederholt benötigt). Wenn möglich, greifen Sie bitte immer sequenziell auf die Daten zu (Zeile für Zeile). |
| Wenn die Daten einer Zeile/eines Feldes geändert werden, können auch die Daten anderer Zellen/Zeilen beeinflusst werden (z. B. werden Daten verschoben, um ausreichend Platz für die geänderten Daten zu schaffen). Daher erfordert jede Änderung einer Daten­einheit die Synchronisation anderer vorhandener Objekte (wie Zeilen‑ oder Zellenobjekte). Um eine bessere Leistung zu erzielen, sollten Sie nicht gleichzeitig mehrere Zeilen/Zellen pflegen. Die Verarbeitung nacheinander reduziert die Datensynchronisation und verbessert die Leistung. |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


Speicherleistung ist vorzuziehen.

**Remarks**

Mit diesem Modus werden die Zellendaten im kompakten Format gehalten, um die Speicherkosten zu senken. Andererseits kann das kompakte Datenformat auch zu höheren Zeitkosten führen, insbesondere beim Aktualisieren der Zellendaten oder beim zufälligen Zugriff.

Diese Option ist seit v8.0.0 verfügbar.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Standardmodus für das Zellenmodell.

**Remarks**

Dieser Modus wird für alle Versionen angewendet.

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

