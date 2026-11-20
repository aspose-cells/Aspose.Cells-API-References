---
title: "CalculationOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt Optionen für die Berechnung dar."
type: docs
url: /de/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Stellt Optionen für die Berechnung dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | Die Stapelgröße für die rekursive Berechnung von Zellen. |
| [getCalculationMonitor()](#getCalculationMonitor--) | Der Monitor für den Benutzer, um den Fortschritt der Formelberechnung zu verfolgen. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Gibt die Kodierung an, die beim Kodieren/Dekodieren von Zeichen während der Berechnung von Formeln verwendet wird. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | Die benutzerdefinierte Formelberechnungs-Engine, um die Standardberechnungs-Engine von Aspose.Cells zu erweitern. |
| [getIgnoreError()](#getIgnoreError--) | Gibt an, ob bei der Berechnung von Formeln auftretende Fehler ignoriert werden sollen. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Gibt die Datenquellen für externe Links an, die in Formeln verwendet werden. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Gibt die Strategie zur Verarbeitung der Berechnungsgenauigkeit an. |
| [getRecursive()](#getRecursive--) | Gibt an, ob abhängige Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Gibt an, ob dynamische Array-Formeln vor der Berechnung von Formeln aktualisiert werden sollen. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Gibt an, ob der Benutzer das Verhalten der Aktualisierung dynamischer Array-Formeln vor der Berechnung der angegebenen Formeln ausdrücklich festgelegt hat. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | Die Stapelgröße für die rekursive Berechnung von Zellen. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | Der Monitor für den Benutzer, um den Fortschritt der Formelberechnung zu verfolgen. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Gibt die Kodierung an, die beim Kodieren/Dekodieren von Zeichen während der Berechnung von Formeln verwendet wird. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | Die benutzerdefinierte Formelberechnungs-Engine, um die Standardberechnungs-Engine von Aspose.Cells zu erweitern. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Gibt an, ob bei der Berechnung von Formeln auftretende Fehler ignoriert werden sollen. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Gibt die Datenquellen für externe Links an, die in Formeln verwendet werden. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Gibt die Strategie zur Verarbeitung der Berechnungsgenauigkeit an. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Gibt an, ob abhängige Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Gibt an, ob dynamische Array-Formeln vor der Berechnung von Formeln aktualisiert werden sollen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
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
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


Die Stapelgröße für die rekursive Berechnung von Zellen. Der Standardwert ist 200.

**Remarks**

Wenn eine große Anzahl von Zellen im Abhängigkeitsbaum rekursiv berechnet werden muss, kann im Berechnungsprozess eine StackOverflowException auftreten. In diesem Fall sollte der Benutzer für diese Eigenschaft einen kleineren Wert angeben. Für solche Situationen sollte der Benutzer den geeigneten Wert für diese Eigenschaft anhand der tatsächlichen Formeln und Daten bestimmen. Ein zu kleiner Wert kann jedoch die Leistungsfähigkeit der Formelb berechnung beeinträchtigen, und ein Wert kleiner als 2 macht es unmöglich, eine Formel zu berechnen, die von einer anderen abhängt. Daher wird ein angegebener Wert kleiner als 2 auf 2 zurückgesetzt.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


Der Monitor für den Benutzer, um den Fortschritt der Formelberechnung zu verfolgen.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Legt die Kodierung fest, die beim Kodieren/Dekodieren von Zeichen während der Berechnung von Formeln verwendet wird. Für Funktionen wie CHAR, CODE hängt das berechnete Ergebnis von den Regionseinstellungen und dem Standard‑Zeichensatz der Umgebung ab. Mit dieser Eigenschaft kann der Benutzer die für diese Funktionen zu verwendende passende Kodierung angeben, um das erwartete Ergebnis zu erhalten.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


Die benutzerdefinierte Formelberechnungs-Engine, um die Standardberechnungs-Engine von Aspose.Cells zu erweitern.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Gibt an, ob bei der Berechnung von Formeln auftretende Fehler ignoriert werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein. Der Standardwert ist true.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Gibt die Datenquellen für externe Links an, die in Formeln verwendet werden.

**Remarks**

Wie bei [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) können Sie hier Datenquellen für externe Links angeben, die in Formeln verwendet und berechnet werden sollen, insbesondere solche, die in der INDIRECT‑Funktion verwendet werden. Für diese externen Links, die in der INDIRECT‑Funktion verwendet werden, werden sie nicht als Teil der externen Links der Arbeitsmappe betrachtet und können nicht mit [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) aktualisiert werden. Die Zuordnung dieser Arbeitsmappen zu externen Links wird durch [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) und [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) bestimmt. Stellen Sie daher sicher, dass [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) den richtigen Wert hat (in der Regel sollte er mit dem entsprechenden [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) übereinstimmen) für jede Arbeitsmappe, damit sie wie erwartet verknüpft werden können.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Gibt die Strategie zur Verarbeitung der Berechnungsgenauigkeit an.

Siehe [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Gibt an, ob die abhängigen Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. Der Standardwert ist true.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


Gibt an, ob dynamische Array-Formeln vor der Berechnung von Formeln aktualisiert werden sollen.

**Remarks**

Wenn diese Eigenschaft explizit angegeben wurde, wird der angegebene Wert verwendet, um zu bestimmen, ob dynamische Array‑Formeln aktualisiert werden sollen. Andernfalls ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) ist falsch), hängt der Standardwert davon ab, welche Art von Formeln berechnet werden muss: Für die Berechnung von Formeln für die Arbeitsmappe, wie z. B. [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), wird diese Eigenschaft als true angenommen. Für andere Fälle, wie z. B. [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) oder [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), wird diese Eigenschaft als false angenommen.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


Gibt an, ob der Benutzer das Verhalten der Aktualisierung dynamischer Array-Formeln vor der Berechnung der angegebenen Formeln ausdrücklich festgelegt hat.

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




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


Die Stapelgröße für die rekursive Berechnung von Zellen. Der Standardwert ist 200.

**Remarks**

Wenn eine große Anzahl von Zellen im Abhängigkeitsbaum rekursiv berechnet werden muss, kann im Berechnungsprozess eine StackOverflowException auftreten. In diesem Fall sollte der Benutzer für diese Eigenschaft einen kleineren Wert angeben. Für solche Situationen sollte der Benutzer den geeigneten Wert für diese Eigenschaft anhand der tatsächlichen Formeln und Daten bestimmen. Ein zu kleiner Wert kann jedoch die Leistungsfähigkeit der Formelb berechnung beeinträchtigen, und ein Wert kleiner als 2 macht es unmöglich, eine Formel zu berechnen, die von einer anderen abhängt. Daher wird ein angegebener Wert kleiner als 2 auf 2 zurückgesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


Der Monitor für den Benutzer, um den Fortschritt der Formelberechnung zu verfolgen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Legt die Kodierung fest, die beim Kodieren/Dekodieren von Zeichen während der Berechnung von Formeln verwendet wird. Für Funktionen wie CHAR, CODE hängt das berechnete Ergebnis von den Regionseinstellungen und dem Standard‑Zeichensatz der Umgebung ab. Mit dieser Eigenschaft kann der Benutzer die für diese Funktionen zu verwendende passende Kodierung angeben, um das erwartete Ergebnis zu erhalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


Die benutzerdefinierte Formelberechnungs-Engine, um die Standardberechnungs-Engine von Aspose.Cells zu erweitern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Gibt an, ob bei der Berechnung von Formeln auftretende Fehler ignoriert werden sollen. Der Fehler kann eine nicht unterstützte Funktion, externe Links usw. sein. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Gibt die Datenquellen für externe Links an, die in Formeln verwendet werden.

**Remarks**

Wie bei [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) können Sie hier Datenquellen für externe Links angeben, die in Formeln verwendet und berechnet werden sollen, insbesondere solche, die in der INDIRECT‑Funktion verwendet werden. Für diese externen Links, die in der INDIRECT‑Funktion verwendet werden, werden sie nicht als Teil der externen Links der Arbeitsmappe betrachtet und können nicht mit [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) aktualisiert werden. Die Zuordnung dieser Arbeitsmappen zu externen Links wird durch [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) und [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) bestimmt. Stellen Sie daher sicher, dass [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) den richtigen Wert hat (in der Regel sollte er mit dem entsprechenden [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) übereinstimmen) für jede Arbeitsmappe, damit sie wie erwartet verknüpft werden können.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Gibt die Strategie zur Verarbeitung der Berechnungsgenauigkeit an.

Siehe [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Gibt an, ob die abhängigen Zellen rekursiv berechnet werden sollen, wenn eine Zelle berechnet wird und von anderen Zellen abhängt. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


Gibt an, ob dynamische Array-Formeln vor der Berechnung von Formeln aktualisiert werden sollen.

**Remarks**

Wenn diese Eigenschaft explizit angegeben wurde, wird der angegebene Wert verwendet, um zu bestimmen, ob dynamische Array‑Formeln aktualisiert werden sollen. Andernfalls ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) ist falsch), hängt der Standardwert davon ab, welche Art von Formeln berechnet werden muss: Für die Berechnung von Formeln für die Arbeitsmappe, wie z. B. [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), wird diese Eigenschaft als true angenommen. Für andere Fälle, wie z. B. [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) oder [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), wird diese Eigenschaft als false angenommen.

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

