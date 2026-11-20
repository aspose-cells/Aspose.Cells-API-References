---
title: "AbstractCalculationMonitor"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Überwacht für den Benutzer den Fortschritt der Formelberechnung."
type: docs
url: /de/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

Überwacht für den Benutzer den Fortschritt der Formelberechnung.

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | Implementieren Sie diese Methode, um nach der Berechnung einer Zelle Geschäftslogik auszuführen. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | Implementieren Sie diese Methode, um vor der Berechnung einer Zelle Geschäftslogik auszuführen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Liefert den neu berechneten Wert der Zelle. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | Liefert den alten Wert der berechneten Zelle. |
| [getValueChanged()](#getValueChanged--) | Ob der Zellenwert nach der Berechnung geändert wurde. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | Implementieren Sie diese Methode, um bei der Berechnung von Formeln mit zirkulären Verweisen Geschäftslogik auszuführen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implementieren Sie diese Methode, um nach der Berechnung einer Zelle Geschäftslogik auszuführen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Index des Arbeitsblatts, zu dem die Zelle gehört. |
| rowIndex | int | Zeilenindex der Zelle |
| colIndex | int | Spaltenindex der Zelle |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implementieren Sie diese Methode, um vor der Berechnung einer Zelle Geschäftslogik auszuführen.

**Remarks**

Für Zellen in Array-Formeln kann diese Methode möglicherweise nicht ausgeführt werden, da diese Zellen in der Regel zusammen berechnet werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Index des Arbeitsblatts, zu dem die Zelle gehört. |
| rowIndex | int | Zeilenindex der Zelle |
| colIndex | int | Spaltenindex der Zelle |

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


Liefert den neu berechneten Wert der Zelle. Sollte nur in [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) verwendet werden.

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


Liefert den alten Wert der berechneten Zelle. Sollte nur in [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) und [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) verwendet werden.

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


Ob der Wert der Zelle nach der Berechnung geändert wurde. Sollte nur in [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-) verwendet werden.

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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


Implementieren Sie diese Methode, um bei der Berechnung von Formeln mit zirkulären Verweisen Geschäftslogik auszuführen.

**Remarks**

In der Implementierung kann der Benutzer außerdem den erwarteten Wert als Berechnungsergebnis für einen Teil/alle dieser Zellen festlegen, sodass die Formelumgebung sie nicht rekursiv berechnet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator mit [CalculationCell](../../com.aspose.cells/calculationcell)-Elementen, die Zellen darstellen, die von zirkulären Verweisen abhängen. |

**Returns:**
boolean - Ob die Formelumgebung diese Zellen nach diesem Aufruf zirkulär berechnen muss. True, damit die Formelumgebung die Berechnung für sie fortsetzt. False, damit die Formelumgebung diese Zellen lediglich als Calculated markiert.
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

