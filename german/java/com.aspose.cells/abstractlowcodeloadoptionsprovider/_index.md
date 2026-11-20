---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Implementierung zur Bereitstellung mehrerer Ladeoptionen für Prozesse, die mehrere Eingaben wie Vorlagendateien verwenden."
type: docs
url: /de/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

Implementierung zur Bereitstellung mehrerer Ladeoptionen für Prozesse, die mehrere Eingaben verwenden (wie z. B. Vorlagendateien).

**Remarks**

Beispielsweise erfordert die Funktion [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) mehrere Vorlagendateien zum Zusammenführen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | Gibt Ressourcen nach der Verarbeitung des aktuellen Eingabeteils frei. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | Ermittelt die Ladeoptionen, aus denen die Daten des aktuell verarbeiteten Teils geladen werden. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | Prüft, ob weitere Eingaben vorhanden sind. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
```


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
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


Gibt Ressourcen nach der Verarbeitung des aktuellen Eingabeteils frei.

**Remarks**

Standardmäßig schließt diese Methode lediglich den durch [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) angegebenen Stream direkt (wenn die Ladeoptionen einen Stream als Quelle angegeben haben). Der Benutzer kann diese Methode überschreiben, um die Freigabe von Ressourcen gemäß seinen Anforderungen und der Implementierung von [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--) zu steuern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | die Ladeoptionen, die für den aktuell aufgeteilten Teil verwendet werden. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```


Ermittelt die Ladeoptionen, aus denen die Daten des aktuell verarbeiteten Teils geladen werden.

**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```


Prüft, ob weitere Eingaben vorhanden sind.

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

