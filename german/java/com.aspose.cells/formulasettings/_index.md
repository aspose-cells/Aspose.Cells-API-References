---
title: "FormulaSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Einstellungen für Formeln und Berechnungen."
type: docs
url: /de/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Einstellungen für Formeln und Berechnungen.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll. |
| [getCalculationId()](#getCalculationId--) | Gibt die Version der Berechnungs‑Engine an, die zur Berechnung von Werten in der Arbeitsmappe verwendet wird. |
| [getCalculationMode()](#getCalculationMode--) | Ermittelt den Modus für die Arbeitsmappenberechnung in MS Excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Gibt an, ob die iterative Berechnung zur Auflösung zirkulärer Verweise aktiviert werden soll. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden. |
| [getMaxChange()](#getMaxChange--) | Die maximale Änderung zur Auflösung eines zirkulären Verweises. |
| [getMaxIteration()](#getMaxIteration--) | Die maximale Anzahl von Durchläufen zur Auflösung eines zirkulären Verweises. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Gibt an, ob die Genauigkeit des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Abrufen und Setzen von Formeln erhalten bleiben sollen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | Gibt die Version der Berechnungs‑Engine an, die zur Berechnung von Werten in der Arbeitsmappe verwendet wird. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Legt den Modus für die Arbeitsmappenberechnung in MS Excel fest. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | Gibt an, ob die iterative Berechnung zur Auflösung zirkulärer Verweise aktiviert werden soll. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden. |
| [setMaxChange(double value)](#setMaxChange-double-) | Die maximale Änderung zur Auflösung eines zirkulären Verweises. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Die maximale Anzahl von Durchläufen zur Auflösung eines zirkulären Verweises. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Gibt an, ob die Genauigkeit des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Abrufen und Setzen von Formeln erhalten bleiben sollen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden der resultierenden Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden und Manipulieren der resultierenden Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Gibt die Version der Berechnungs‑Engine an, die zur Berechnung von Werten in der Arbeitsmappe verwendet wird.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden und Manipulieren der resultierenden Datei entsprechend reagieren können. Im Fall von MS Excel, wenn der Wert dieser Eigenschaft kleiner ist als der Identifier der Neuberechnungs‑Engine, die mit der Anwendung verknüpft ist, die die resultierende Datei öffnet, wird die Anwendung die Ergebnisse aller Formeln in dieser Arbeitsmappe sofort nach dem Laden der Datei neu berechnen. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


Ermittelt den Modus für die Arbeitsmappenberechnung in MS Excel.

Siehe [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellendatei, damit andere Anwendungen (wie ms excel) beim Laden und Verarbeiten der resultierenden Datei entsprechend handeln können. Aus Performance‑Überlegungen für die meisten Benutzeranwendungen berechnen wir keine Formeln im Arbeitsbuch automatisch, unabhängig davon, welcher Modus für diese Eigenschaft festgelegt wurde. Wenn der Benutzer Formeln berechnen muss, rufen Sie bitte stets die Methoden auf verschiedenen Objekten gemäß den Anforderungen auf: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. Standard ist false.

**Remarks**

Wenn im Arbeitsbuch viele Formeln vorhanden sind und der Benutzer sie wiederholt berechnen muss, wobei nur ein kleiner Teil davon geändert wird, kann das Aktivieren der Berechnungskette die Leistung verbessern. Andererseits erfordert die Aufrechterhaltung des Kettenmodells bei aktivierter Kette zusätzlichen Speicher und verbraucht etwas mehr CPU‑Zeit für andere Vorgänge wie das Ändern von Zellwerten oder Formeln. Nachdem diese Eigenschaft von false auf true geändert wurde, wird die Berechnungskette beim ersten Berechnen des Arbeitsbuchs analysiert und aufgebaut, sodass die für die erste Berechnung benötigte Zeit länger sein kann als bei einer normalen Berechnung ohne Kette.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Gibt an, ob die iterative Berechnung zur Auflösung zirkulärer Verweise aktiviert werden soll.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden und Manipulieren der resultierenden Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


Die maximale Änderung zur Auflösung eines zirkulären Verweises.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Die maximale Anzahl von Durchläufen zur Auflösung eines zirkulären Verweises.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Gibt an, ob die Genauigkeit des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben sollen. Standardwert ist false.

**Remarks**

Im Allgemeinen dienen diese Leerzeichen und Zeilenumbrüche nur der visuellen Darstellung; ihr Beibehalten oder Nicht‑Beibehalten beeinflusst das Berechnungsergebnis nicht. Aus Performance‑Gründen, wenn keine besonderen Anforderungen bestehen, ist es besser, sie beim Verarbeiten von Formeln nicht zu erhalten.

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


Gibt an, ob die Anwendung beim Öffnen der Arbeitsmappe eine vollständige Berechnung durchführen muss.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden der resultierenden Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


Gibt an, ob die Arbeitsmappe im manuellen Berechnungsmodus vor dem Speichern des Dokuments neu berechnet werden soll.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden und Manipulieren der resultierenden Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


Gibt die Version der Berechnungs‑Engine an, die zur Berechnung von Werten in der Arbeitsmappe verwendet wird.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden und Manipulieren der resultierenden Datei entsprechend reagieren können. Im Fall von MS Excel, wenn der Wert dieser Eigenschaft kleiner ist als der Identifier der Neuberechnungs‑Engine, die mit der Anwendung verknüpft ist, die die resultierende Datei öffnet, wird die Anwendung die Ergebnisse aller Formeln in dieser Arbeitsmappe sofort nach dem Laden der Datei neu berechnen. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


Legt den Modus für die Arbeitsmappenberechnung in MS Excel fest.

Siehe [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellendatei, damit andere Anwendungen (wie ms excel) beim Laden und Verarbeiten der resultierenden Datei entsprechend handeln können. Aus Performance‑Überlegungen für die meisten Benutzeranwendungen berechnen wir keine Formeln im Arbeitsbuch automatisch, unabhängig davon, welcher Modus für diese Eigenschaft festgelegt wurde. Wenn der Benutzer Formeln berechnen muss, rufen Sie bitte stets die Methoden auf verschiedenen Objekten gemäß den Anforderungen auf: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


Gibt an, ob die Berechnungskette für Formeln aktiviert werden soll. Standard ist false.

**Remarks**

Wenn im Arbeitsbuch viele Formeln vorhanden sind und der Benutzer sie wiederholt berechnen muss, wobei nur ein kleiner Teil davon geändert wird, kann das Aktivieren der Berechnungskette die Leistung verbessern. Andererseits erfordert die Aufrechterhaltung des Kettenmodells bei aktivierter Kette zusätzlichen Speicher und verbraucht etwas mehr CPU‑Zeit für andere Vorgänge wie das Ändern von Zellwerten oder Formeln. Nachdem diese Eigenschaft von false auf true geändert wurde, wird die Berechnungskette beim ersten Berechnen des Arbeitsbuchs analysiert und aufgebaut, sodass die für die erste Berechnung benötigte Zeit länger sein kann als bei einer normalen Berechnung ohne Kette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


Gibt an, ob die iterative Berechnung zur Auflösung zirkulärer Verweise aktiviert werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


Gibt an, ob bei jeder Auslösung einer Berechnung alle Formeln neu berechnet werden.

**Remarks**

Diese Eigenschaft dient ausschließlich dem Speichern der Einstellungen in die resultierende Tabellenkalkulationsdatei, damit andere Anwendungen (wie MS Excel) beim Laden und Manipulieren der resultierenden Datei entsprechend reagieren können. Aus Leistungsgründen für die meisten Benutzeranwendungen berechnen wir keine Formel in der Arbeitsmappe automatisch, unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


Die maximale Änderung zur Auflösung eines zirkulären Verweises.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Die maximale Anzahl von Durchläufen zur Auflösung eines zirkulären Verweises.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Gibt an, ob die Genauigkeit des berechneten Ergebnisses so festgelegt wird, wie sie bei der Berechnung von Formeln angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Gibt an, ob die zwischen Formel‑Token eingefügten Leerzeichen und Zeilenumbrüche beim Abrufen und Setzen von Formeln erhalten bleiben sollen. Standardwert ist false.

**Remarks**

Im Allgemeinen dienen diese Leerzeichen und Zeilenumbrüche nur der visuellen Darstellung; ihr Beibehalten oder Nicht‑Beibehalten beeinflusst das Berechnungsergebnis nicht. Aus Performance‑Gründen, wenn keine besonderen Anforderungen bestehen, ist es besser, sie beim Verarbeiten von Formeln nicht zu erhalten.

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

