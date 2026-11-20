---
title: "GridAbstractCalculationEngine"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die benutzerdefinierte Berechnungs-Engine des Benutzers dar, um die Standard-Berechnungs-Engine von Aspose.Cells zu erweitern."
type: docs
url: /de/java/com.aspose.gridjs/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

Stellt die benutzerdefinierte Berechnungs‑Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern.

**Remarks**

Der Benutzer sollte keinen Teil der Arbeitsmappe in dieser Implementierung direkt ändern (außer dem berechneten Ergebnis der benutzerdefinierten Funktion, das über die Eigenschaft GridCalculationData.CalculatedValue festgelegt werden kann). Andernfalls können unerwartete Ergebnisse oder Ausnahmen auftreten. Wenn der Benutzer andere Daten als das berechnete Ergebnis in der Implementierung für einige benutzerdefinierte Funktionen ändern muss, z. B. die Formel einer Zelle, den Stil usw., sollte er diese Daten in dieser Implementierung sammeln und außerhalb des Bereichs der Formelb berechnung ändern.

**Example**

```
          class MyEngine extends GridAbstractCalculationEngine
         {
             public /*override*/ void calculate(GridCalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {   
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof GridReferredArea)
                         {
                             GridReferredArea ra = (GridReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridjs.GridCalculationData-) | Berechnet eine Funktion mit den angegebenen Daten. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```


### calculate(GridCalculationData data) {#calculate-com.aspose.gridjs.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


Berechnet eine Funktion mit den angegebenen Daten.

**Remarks**

Der Benutzer sollte den berechneten Wert für die angegebenen Daten für alle Funktionen (einschließlich Excel-nativer Funktionen) festlegen, die er in dieser Implementierung selbst berechnen möchte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridjs/gridcalculationdata) | Die erforderlichen Daten zur Berechnung einer Funktion, wie Funktionsname, Parameter usw. |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

