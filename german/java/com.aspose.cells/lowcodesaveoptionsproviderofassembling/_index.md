---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern, und der Pfad der resultierenden Datei wird benannt, da er Verzeichnisse wie SheetIndex oder SheetName SplitPartIndex enthalten kann."
type: docs
url: /de/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern, und der Pfad der resultierenden Datei wird benannt (er kann Verzeichnisse enthalten): [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(oder SheetName) +[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Gibt Ressourcen nach der Verarbeitung des aktuell geteilten Teils frei. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Ob der Split‑Part‑Index immer zum Dateipfad hinzugefügt wird. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | Kopfteil (vor dem hinzugefügten Inhalt von Blatt und Split‑Part) des Dateipfads. |
| [getPathTail()](#getPathTail--) | Endteil (nach den Sequenznummern) des Dateipfads. |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Ermittelt die Speicheroptionen, aus denen die Ausgabeeinstellungen für den aktuell geteilten Teil abgerufen werden. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Versatz des Blattindexes zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | Präfix für den Index des Arbeitsblatts. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Versatz des Index des geteilten Teils zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Präfix für den Index des geteilten Teils. |
| [getUseSheetName()](#getUseSheetName--) | Ob der Dateipfad mit Blattnamen statt Blattindex erstellt wird. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Ob der Split‑Part‑Index immer zum Dateipfad hinzugefügt wird. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | Kopfteil (vor dem hinzugefügten Inhalt von Blatt und Split‑Part) des Dateipfads. |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | Endteil (nach den Sequenznummern) des Dateipfads. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Versatz des Blattindexes zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | Präfix für den Index des Arbeitsblatts. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Versatz des Index des geteilten Teils zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Präfix für den Index des geteilten Teils. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | Ob der Dateipfad mit Blattnamen statt Blattindex erstellt wird. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
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

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein Blatt vorhanden ist, werden der Blattindex (oder Name) und das entsprechende Präfix nicht zum Dateipfad hinzugefügt.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein geteiltes Teil vorhanden ist, werden der Index des geteilten Teils und das entsprechende Präfix nicht zum Dateipfad hinzugefügt.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


Kopfteil (vor dem hinzugefügten Inhalt von Blatt und Split‑Part) des Dateipfads.

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


Nachgestellter Teil (nach den Sequenznummern) des Dateipfads. Er sollte die Dateierweiterung enthalten.

**Returns:**
java.lang.String
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Ermittelt die Speicheroptionen, aus denen die Ausgabeeinstellungen für den aktuell geteilten Teil abgerufen werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Wenn die Vorlage angegeben wurde, kopiert die erstellte Instanz alle Einstellungen daraus und aktualisiert die Ausgabedatei entsprechend.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Versatz des Blattindexes zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Wirkt nur, wenn [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) false ist.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


Präfix für den Index des Arbeitsblatts.

**Remarks**

Wenn nur ein Arbeitsblatt vorhanden ist und [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) false ist, werden dieses Präfix und der Blattindex (oder Name) nicht zum resultierenden Dateipfad hinzugefügt.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


Versatz des Index des geteilten Teils zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


Präfix für den Index des geteilten Teils.

**Remarks**

Wenn nur ein geteiltes Teil vorhanden ist und [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) false ist, werden dieses Präfix und der Index des geteilten Teils (0) nicht zum resultierenden Dateipfad hinzugefügt.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


Ob der Dateipfad mit Blattnamen statt Blattindex erstellt wird. Der Standardwert ist false.

**Remarks**

Der Blattname wird niemals automatisch neu erstellt. Wenn er also auf true gesetzt wird, stellen Sie bitte sicher, dass kein spezieller Blattname vorhanden ist, der einen ungültigen Dateipfad oder -namen verursachen kann.

**Returns:**
boolean
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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein Blatt vorhanden ist, werden der Blattindex (oder Name) und das entsprechende Präfix nicht zum Dateipfad hinzugefügt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein geteiltes Teil vorhanden ist, werden der Index des geteilten Teils und das entsprechende Präfix nicht zum Dateipfad hinzugefügt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


Kopfteil (vor dem hinzugefügten Inhalt von Blatt und Split‑Part) des Dateipfads.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


Nachgestellter Teil (nach den Sequenznummern) des Dateipfads. Er sollte die Dateierweiterung enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Wenn die Vorlage angegeben wurde, kopiert die erstellte Instanz alle Einstellungen daraus und aktualisiert die Ausgabedatei entsprechend.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


Versatz des Blattindexes zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Wirkt nur, wenn [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) false ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


Präfix für den Index des Arbeitsblatts.

**Remarks**

Wenn nur ein Arbeitsblatt vorhanden ist und [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) false ist, werden dieses Präfix und der Blattindex (oder Name) nicht zum resultierenden Dateipfad hinzugefügt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


Versatz des Index des geteilten Teils zwischen dem, was im Dateipfad verwendet wird, und seinem tatsächlichen Wert ([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


Präfix für den Index des geteilten Teils.

**Remarks**

Wenn nur ein geteiltes Teil vorhanden ist und [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) false ist, werden dieses Präfix und der Index des geteilten Teils (0) nicht zum resultierenden Dateipfad hinzugefügt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


Ob der Dateipfad mit Blattnamen statt Blattindex erstellt wird. Der Standardwert ist false.

**Remarks**

Der Blattname wird niemals automatisch neu erstellt. Wenn er also auf true gesetzt wird, stellen Sie bitte sicher, dass kein spezieller Blattname vorhanden ist, der einen ungültigen Dateipfad oder -namen verursachen kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

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

