---
title: "GridWorkbookSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Einstellungen der Arbeitsmappe dar."
type: docs
url: /de/java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Stellt die Einstellungen der Arbeitsmappe dar.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Liefert den Autor der Datei. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird, Standard ist false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Gibt an, ob eine Kette berechneter Formeln erstellt wird. |
| [getDate1904()](#getDate1904--) | Liefert einen Wert, der angibt, ob das Arbeitsbuch das 1904-Datumsystem verwendet. |
| [getEnableMacros()](#getEnableMacros--) | Makros aktivieren; funktioniert derzeit nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt innerhalb einer Arbeitsmappe. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Gibt an, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird. |
| [getIteration()](#getIteration--) | Gibt an, ob Iteration verwendet wird, um zirkuläre Verweise aufzulösen. |
| [getMaxIteration()](#getMaxIteration--) | Gibt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises zurück oder legt sie fest, der Standardwert ist 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Gibt an, ob beim Öffnen der Datei alle Formeln neu berechnet werden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Legt den Autor der Datei fest. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird, Standard ist false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Gibt an, ob eine Kette berechneter Formeln erstellt wird. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Legt einen Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Makros aktivieren; funktioniert derzeit nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt innerhalb einer Arbeitsmappe. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Gibt an, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird. |
| [setIteration(boolean value)](#setIteration-boolean-) | Gibt an, ob Iteration verwendet wird, um zirkuläre Verweise aufzulösen. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Gibt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises zurück oder legt sie fest, der Standardwert ist 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Gibt an, ob beim Öffnen der Datei alle Formeln neu berechnet werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
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


Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird, Standard ist false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB, z. B. über Cell.PutValue(string), eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir den eingegebenen Zeichenfolgenwert als Zellwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festgelegt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. Standard ist false.

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


Gibt an, ob eine Kette berechneter Formeln erstellt wird. Standard ist false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Liefert einen Wert, der angibt, ob das Arbeitsbuch das 1904-Datumsystem verwendet.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Makros aktivieren; funktioniert derzeit nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt innerhalb einer Arbeitsmappe.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Gibt an, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Gibt an, ob Iteration verwendet wird, um zirkuläre Verweise aufzulösen.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Gibt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises zurück oder legt sie fest, der Standardwert ist 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


True, wenn Berechnungen in dieser Arbeitsmappe nur mit der Genauigkeit der angezeigten Zahlen durchgeführt werden

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Gibt an, ob beim Öffnen der Datei alle Formeln neu berechnet werden. Standard ist true.

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


Gibt an, ob beim Festlegen von Style.Custom das benutzerdefinierte Zahlenformat überprüft wird, Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB, z. B. über Cell.PutValue(string), eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, akzeptieren wir den eingegebenen Zeichenfolgenwert als Zellwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festgelegt haben, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Gibt an, ob eine Kette berechneter Formeln erstellt wird. Standard ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Legt einen Wert fest, der angibt, ob die Arbeitsmappe das 1904-Datumsystem verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Makros aktivieren; funktioniert derzeit nur beim Kopieren eines Arbeitsblatts in ein anderes Arbeitsblatt innerhalb einer Arbeitsmappe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Gibt an, ob bei jeder Auslösung einer Berechnung vollständig neu berechnet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Gibt an, ob Iteration verwendet wird, um zirkuläre Verweise aufzulösen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Gibt die maximale Anzahl von Iterationen zur Auflösung eines zirkulären Verweises zurück oder legt sie fest, der Standardwert ist 100.

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

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Gibt an, ob beim Öffnen der Datei alle Formeln neu berechnet werden. Standard ist true.

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

