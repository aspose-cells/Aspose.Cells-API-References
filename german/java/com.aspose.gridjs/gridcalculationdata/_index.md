---
title: "GridCalculationData"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die erforderlichen Daten dar, die beim Berechnen einer Funktion benötigt werden, wie Funktionsname, Parameter …usw."
type: docs
url: /de/java/com.aspose.gridjs/gridcalculationdata/
---

**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```

Stellt die erforderlichen Daten bei der Berechnung einer Funktion dar, wie Funktionsname, Parameter, …usw.

**Remarks**

Alle von dieser Klasse bereitgestellten Objekte dienen ausschließlich dem \"Lese\"-Zweck. Der Benutzer sollte während des Formelberechnungsprozesses keine Daten im Workbook ändern, da sonst unerwartete Ergebnisse oder Ausnahmen auftreten können.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Liefert den berechneten Wert für diese Funktion. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gibt den Spaltenindex der Zelle zurück, in der sich die Funktion befindet. |
| [getFormula()](#getFormula--) | Gibt die Zellformel zurück, in der sich die Funktion befindet. |
| [getFunctionName()](#getFunctionName--) | Liefert den Funktionsnamen, der berechnet werden soll. |
| [getParamCount()](#getParamCount--) | Gibt die Anzahl der Parameter zurück. |
| [getParamText(int index)](#getParamText-int-) | Gibt den wörtlichen Text des Parameters am angegebenen Index zurück. |
| [getParamValue(int index)](#getParamValue-int-) | Liefert das dargestellte Wertobjekt des Parameters am angegebenen Index. |
| [getRow()](#getRow--) | Liefert den Zeilenindex der Zelle, in der sich die Funktion befindet. |
| [getSheetName()](#getSheetName--) | Liefert den Arbeitsblattnamen, in dem sich die Funktion befindet. |
| [getStringValue()](#getStringValue--) | Liefert den Anzeigestringwert der Zelle, in der sich die Funktion befindet. |
| [getValue()](#getValue--) | Liefert den Zellenwert, in dem sich die Funktion befindet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Setzt den berechneten Wert für diese Funktion. |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Liefert den berechneten Wert für diese Funktion.

**Remarks**

Der Benutzer sollte diese Eigenschaft in seiner benutzerdefinierten Berechnungs-Engine für die von der Engine unterstützten Funktionen setzen, und der gesetzte Wert wird beim Abrufen dieser Eigenschaft zurückgegeben. Das Abrufen dieser Eigenschaft, bevor sie gesetzt wurde, führt dazu, dass die Funktion von der Standard-Berechnungs-Engine von Aspose.Cells berechnet wird und der berechnete Wert zurückgegeben wird.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Gibt den Spaltenindex der Zelle zurück, in der sich die Funktion befindet.

**Returns:**
int
### getFormula() {#getFormula--}
```
public String getFormula()
```


Gibt die Zellformel zurück, in der sich die Funktion befindet.

**Returns:**
java.lang.String
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


Liefert den Funktionsnamen, der berechnet werden soll.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


Gibt die Anzahl der Parameter zurück.

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Gibt den wörtlichen Text des Parameters am angegebenen Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des Parameters (0‑basiert). |

**Returns:**
java.lang.String – Der wörtliche Text des Parameters.
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Liefert das dargestellte Wertobjekt des Parameters am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des Parameters (0‑basiert). |

**Returns:**
java.lang.Object – Wenn der Parameter ein einfacher Wert ist, wird der einfache Wert zurückgegeben. Wenn der Parameter eine Referenz ist, wird ein ReferredArea‑Objekt zurückgegeben.
### getRow() {#getRow--}
```
public int getRow()
```


Liefert den Zeilenindex der Zelle, in der sich die Funktion befindet.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Liefert den Arbeitsblattnamen, in dem sich die Funktion befindet.

**Returns:**
java.lang.String
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Liefert den Anzeigestringwert der Zelle, in der sich die Funktion befindet.

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Liefert den Zellenwert, in dem sich die Funktion befindet.

**Returns:**
java.lang.Object
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


Setzt den berechneten Wert für diese Funktion.

**Remarks**

Der Benutzer sollte diese Eigenschaft in seiner benutzerdefinierten Berechnungs-Engine für die von der Engine unterstützten Funktionen setzen, und der gesetzte Wert wird beim Abrufen dieser Eigenschaft zurückgegeben. Das Abrufen dieser Eigenschaft, bevor sie gesetzt wurde, führt dazu, dass die Funktion von der Standard-Berechnungs-Engine von Aspose.Cells berechnet wird und der berechnete Wert zurückgegeben wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

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

