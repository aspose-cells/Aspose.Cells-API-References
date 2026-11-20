---
title: "CalculationData"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die erforderlichen Daten dar, die beim Berechnen einer Funktion benötigt werden, wie Funktionsname, Parameter …usw."
type: docs
url: /de/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

Stellt die erforderlichen Daten bei der Berechnung einer Funktion dar, wie Funktionsname, Parameter, …usw.

**Remarks**

Alle von dieser Klasse bereitgestellten Objekte dienen ausschließlich dem \"Lese\"-Zweck. Der Benutzer sollte während des Formelberechnungsprozesses keine Daten im Workbook ändern, da sonst unerwartete Ergebnisse oder Ausnahmen auftreten können.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Liefert den berechneten Wert für diese Funktion. |
| [getCell()](#getCell--) | Liefert das Cell-Objekt, in dem sich die Funktion befindet. |
| [getCellColumn()](#getCellColumn--) | Liefert den Spaltenindex der Zelle, in der sich die Funktion befindet. |
| [getCellRow()](#getCellRow--) | Liefert den Zeilenindex der Zelle, in der sich die Funktion befindet. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Liefert den Funktionsnamen, der berechnet werden soll. |
| [getParamCount()](#getParamCount--) | Liefert die Anzahl der Parameter |
| [getParamText(int index)](#getParamText-int-) | Liefert den wörtlichen Text des Parameters am angegebenen Index. |
| [getParamValue(int index)](#getParamValue-int-) | Liefert das dargestellte Wertobjekt des Parameters an einem angegebenen Index. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | Liefert den/die Wert(e) des Parameters an einem angegebenen Index. |
| [getWorkbook()](#getWorkbook--) | Liefert das Workbook-Objekt, in dem sich die Funktion befindet. |
| [getWorksheet()](#getWorksheet--) | Liefert das Worksheet-Objekt, in dem sich die Funktion befindet. |
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

Der Benutzer sollte diese Eigenschaft in seiner benutzerdefinierten Berechnungs-Engine für die von der Engine unterstützten Funktionen setzen, und der gesetzte Wert wird später beim Abrufen dieser Eigenschaft zurückgegeben. Der gesetzte Wert kann von möglichen Typen sein, wie [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), ein Array solcher Werte oder ein Range, Name, ReferredArea. Das Abrufen dieser Eigenschaft, bevor ein Wert gesetzt wurde, führt dazu, dass die Funktion von der Standard‑Berechnungs‑Engine von Aspose.Cells berechnet wird und dann der berechnete Wert zurückgegeben wird (in der Regel sollte es \#NAME? für benutzerdefinierte Funktionen sein).

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


Liefert das Cell-Objekt, in dem sich die Funktion befindet.

**Remarks**

Beim Berechnen einer Formel, ohne sie einer Zelle zuzuweisen, beispielsweise mittels [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-), wird die Formel so berechnet, als wäre sie in Zelle A1 gesetzt, sodass sowohl [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) als auch [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) 0 sind. Allerdings ist die Zelle A1 im Arbeitsblatt möglicherweise nicht instanziiert. In einem solchen Fall ist diese Eigenschaft also null.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Liefert den Spaltenindex der Zelle, in der sich die Funktion befindet.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Liefert den Zeilenindex der Zelle, in der sich die Funktion befindet.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


Liefert die Anzahl der Parameter

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


Liefert den wörtlichen Text des Parameters am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Index des Parameters (0‑basiert) |

**Returns:**
java.lang.String – wörtlicher Text des Parameters
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


Liefert das dargestellte Wertobjekt des Parameters an einem angegebenen Index.

**Remarks**

Für einen Parameter:

Wenn es ein einfacher Wert ist, wird der einfache Wert selbst zurückgegeben;

Wenn es eine Referenz ist, wird ein ReferredArea‑Objekt zurückgegeben;

Wenn es auf Datensatz(e) mit mehreren Werten verweist, wird ein Array von Objekten zurückgegeben;

Wenn es sich um eine Art Ausdruck handelt, der berechnet werden muss, wird er im Wertmodus berechnet und in der Regel ein einzelner Wert zurückgegeben, basierend auf der aktuellen Zelle. Zum Beispiel, wenn ein Parameter der Formel von D2 A:A+B:B ist, wird A2+B2 berechnet und zurückgegeben. Wird dieser Parameter jedoch als Array‑Modus angegeben (durch  oder ), wird ein Array (object[][]) zurückgegeben, dessen Elemente A1+B1, A2+B2, … sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des Parameters (0‑basiert) |

**Returns:**
java.lang.Object - Der berechnete Wert des Parameters.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


Liefert den/die Wert(e) des Parameters an einem angegebenen Index. Wenn der Parameter eine Art Ausdruck ist, der berechnet werden muss, wird er im Array‑Modus berechnet.

**Remarks**

Für einen Ausdruck, der berechnet werden muss, am Beispiel A:A+B:B: Im Werte‑Modus wird er zu einem einzelnen Wert basierend auf der aktuellen Zellenbasis berechnet. Im Array‑Modus werden jedoch alle Werte von A1+B1, A2+B2, A3+B3, … berechnet und zum Erzeugen des zurückgegebenen Arrays verwendet. In einer solchen Situation ist es besser, die Grenze für die Zeilen‑/Spaltenanzahl anzugeben (z. B. gemäß [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) und [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--)), da sonst das zurückgegebene große Array den Speicherverbrauch durch eine große Menge nutzloser Daten erhöhen kann.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index des Parameters (0‑basiert) |
| maxRowCount | int | Die Zeilenanzahl‑Grenze für das zurückgegebene Array. Ist sie nicht positiv oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Zeilenanzahl verwendet. |
| maxColumnCount | int | Die Spaltenanzahl‑Grenze für das zurückgegebene Array. Ist sie nicht positiv oder größer als die tatsächliche Zeilenanzahl, wird die tatsächliche Spaltenanzahl verwendet. |

**Returns:**
java.lang.Object[][] - Ein Array, das alle durch den angegebenen Parameter dargestellten Elemente enthält.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Liefert das Workbook-Objekt, in dem sich die Funktion befindet.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Liefert das Worksheet-Objekt, in dem sich die Funktion befindet.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

Der Benutzer sollte diese Eigenschaft in seiner benutzerdefinierten Berechnungs-Engine für die von der Engine unterstützten Funktionen setzen, und der gesetzte Wert wird später beim Abrufen dieser Eigenschaft zurückgegeben. Der gesetzte Wert kann von möglichen Typen sein, wie [Cell.getValue()](../../com.aspose.cells/cell\#getValue--), ein Array solcher Werte oder ein Range, Name, ReferredArea. Das Abrufen dieser Eigenschaft, bevor ein Wert gesetzt wurde, führt dazu, dass die Funktion von der Standard‑Berechnungs‑Engine von Aspose.Cells berechnet wird und dann der berechnete Wert zurückgegeben wird (in der Regel sollte es \#NAME? für benutzerdefinierte Funktionen sein).

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

