---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Einstellungen der Arbeitsmappe dar."
type: docs
url: /de/java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Serializable
```
public class GridWorkbookSettings implements Serializable
```

Stellt die Einstellungen der Arbeitsmappe dar.

**Example**

```
         GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
         //do your business
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) | Standardkonstruktor |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Liefert den Autor der Datei. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Ermittelt, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Ermittelt, ob eine berechnete Formelkette erstellt wird. |
| [getDate1904()](#getDate1904--) | Ermittelt den Wert, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet. |
| [getEnableMacros()](#getEnableMacros--) | Ermittelt, ob Makros aktiviert sind; jetzt funktioniert es nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt einer Arbeitsmappe. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Ermittelt, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird. |
| [getIteration()](#getIteration--) | Ermittelt, ob Iterationen zur Auflösung zirkulärer Verweise verwendet werden. |
| [getMaxIteration()](#getMaxIteration--) | Ermittelt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises, der Standardwert ist 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Ermittelt, ob beim Öffnen der Datei alle Formeln neu berechnet werden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Legt den Autor der Datei fest. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Legt fest, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Legt fest, ob eine berechnete Formelkette erstellt wird. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Legt den Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Legt fest, ob Makros aktiviert sind; jetzt funktioniert es nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt einer Arbeitsmappe. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Legt fest, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird. |
| [setIteration(boolean value)](#setIteration-boolean-) | Legt fest, ob Iterationen zur Auflösung zirkulärer Verweise verwendet werden. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Legt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises fest, der Standardwert ist 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben. |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Legt fest, ob beim Öffnen der Datei alle Formeln neu berechnet werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
```


Standardkonstruktor

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Liefert den Autor der Datei.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Ermittelt, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Ermittelt, ob eine berechnete Formelkette erstellt wird. Standard ist false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Ermittelt den Wert, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Ermittelt, ob Makros aktiviert sind; jetzt funktioniert es nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt einer Arbeitsmappe.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Ermittelt, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Ermittelt, ob Iterationen zur Auflösung zirkulärer Verweise verwendet werden.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Ermittelt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises, der Standardwert ist 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Der Standardwert ist false.

**Remarks**

Im Allgemeinen dienen diese Leerzeichen und Zeilenumbrüche nur der visuellen Darstellung; ihr Beibehalten oder Nicht‑Beibehalten beeinflusst das Berechnungsergebnis nicht. Aus Performance‑Gründen, wenn keine besonderen Anforderungen bestehen, ist es besser, sie beim Verarbeiten von Formeln nicht zu erhalten.

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Ermittelt, ob beim Öffnen der Datei alle Formeln neu berechnet werden.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Legt den Autor der Datei fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Legt fest, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Legt fest, ob eine berechnete Formelkette erstellt wird. Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Legt den Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Legt fest, ob Makros aktiviert sind; jetzt funktioniert es nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt einer Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Legt fest, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Legt fest, ob Iterationen zur Auflösung zirkulärer Verweise verwendet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Legt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises fest, der Standardwert ist 100.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln beibehalten werden sollen. Der Standardwert ist false.

**Remarks**

Im Allgemeinen dienen diese Leerzeichen und Zeilenumbrüche nur der visuellen Darstellung; ihr Beibehalten oder Nicht‑Beibehalten beeinflusst das Berechnungsergebnis nicht. Aus Performance‑Gründen, wenn keine besonderen Anforderungen bestehen, ist es besser, sie beim Verarbeiten von Formeln nicht zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Legt fest, ob beim Öffnen der Datei alle Formeln neu berechnet werden.

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

