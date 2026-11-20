---
title: "AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Implementierung zur Bereitstellung mehrerer Speicheroptionen für Prozesse, die mehrere Ausgaben erfordern."
type: docs
url: /de/java/com.aspose.cells/abstractlowcodesaveoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeSaveOptionsProvider
```

Implementierung zur Bereitstellung mehrerer Speicheroptionen für Prozesse, die mehrere Ausgaben erfordern. Zum Beispiel erfordert die Funktion [SpreadsheetSplitter](../../com.aspose.cells/spreadsheetsplitter) mehrere Ziele, um die geteilten Dateien zu speichern.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider()](#AbstractLowCodeSaveOptionsProvider--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Gibt Ressourcen nach der Verarbeitung des aktuell geteilten Teils frei. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Ermittelt die Speicheroptionen, aus denen die Ausgabeeinstellungen für den aktuell geteilten Teil abgerufen werden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeSaveOptionsProvider() {#AbstractLowCodeSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Gibt Ressourcen nach der Verarbeitung des aktuell geteilten Teils frei.

**Remarks**

Standardmäßig schließt diese Methode einfach den von [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) angegebenen Stream direkt (wenn die Speicheroptionen einen Stream als Ziel angegeben haben). Der Benutzer kann diese Methode überschreiben, um zu steuern, wie Ressourcen gemäß seinen Anforderungen freigegeben werden, und die Implementierung von [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-) zu nutzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | die für den aktuell geteilten Teil verwendeten Speicheroptionen. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public abstract LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Ermittelt die Speicheroptionen, aus denen die Ausgabeeinstellungen für den aktuell geteilten Teil abgerufen werden. Die Rückgabe von null bedeutet, den angegebenen Teil zu überspringen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
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

