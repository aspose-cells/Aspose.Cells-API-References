---
title: "AbstractCalculationEngine"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die benutzerdefinierte Berechnungs-Engine des Benutzers dar, um die Standard-Berechnungs-Engine von Aspose.Cells zu erweitern."
type: docs
url: /de/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Stellt die benutzerdefinierte Berechnungs‑Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern.

**Remarks**

Der Benutzer sollte keinen Teil der Arbeitsmappe direkt in dieser Implementierung ändern (außer dem berechneten Ergebnis der benutzerdefinierten Funktion, das über die Eigenschaft CalculationData.CalculatedValue festgelegt werden kann). Andernfalls können unerwartete Ergebnisse oder Exception auftreten. Wenn der Benutzer andere Daten als das berechnete Ergebnis in der Implementierung für einige benutzerdefinierte Funktionen ändern muss, zum Beispiel die Zellformel, den Stil, …etc., sollte er diese Daten in dieser Implementierung sammeln und sie außerhalb des Geltungsbereichs der Formelberechnung ändern.

**Example**

```
         class MyEngine extends AbstractCalculationEngine
         {
             public /*override*/ void calculate(CalculationData data)
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
                         if (pv instanceof ReferredArea)
                         {
                             ReferredArea ra = (ReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
         Workbook wb = new Workbook("custom_calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCustomEngine(new MyEngine());
         wb.calculateFormula(opts);
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Berechnet eine Funktion mit den angegebenen Daten. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Gibt an, ob die gegebene Funktion immer neu berechnet werden soll, wenn gemeinsam genutzte Formeln berechnet werden. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Gibt an, ob integrierte Funktionen, die von der integrierten Engine unterstützt werden, von dieser Implementierung geprüft und verarbeitet werden sollen. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Gibt an, ob diese Engine den Parameter im Array-Modus berechnen muss. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Gibt an, ob diese Engine den wörtlichen Text des Parameters während einer Berechnung benötigt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Überspringt die Berechnung der gesamten Formel, die die derzeit ausgewertete Funktion referenziert. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationEngine() {#AbstractCalculationEngine--}
```
public AbstractCalculationEngine()
```


### calculate(CalculationData data) {#calculate-com.aspose.cells.CalculationData-}
```
public abstract void calculate(CalculationData data)
```


Berechnet eine Funktion mit den angegebenen Daten.

**Remarks**

Der Benutzer sollte den berechneten Wert für die angegebenen Daten für alle Funktionen (einschließlich Excel-nativer Funktionen) festlegen, die er in dieser Implementierung selbst berechnen möchte.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | die erforderlichen Daten zur Berechnung der Funktion, wie Funktionsname, Parameter, …etc. |

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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Gibt an, ob die gegebene Funktion immer neu berechnet werden soll, wenn gemeinsam genutzte Formeln berechnet werden.

**Remarks**

Bei gemeinsam genutzten Formeln teilen mehrere Zellen dieselbe Funktion. Wenn die Parameter der Funktion für diese Zellen ebenfalls gleich bleiben, muss diese Funktion im Allgemeinen nur einmal berechnet werden. Daher berechnen wir aus Leistungsgründen diese Art von Funktion ebenfalls nur einmal ([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) wird nur einmal aufgerufen, anstatt für jede Zelle wiederholt aufgerufen zu werden). Allerdings muss bei einer benutzerdefinierten Implementierung des Benutzers die Funktion, insbesondere die benutzerdefinierte Funktion, möglicherweise für verschiedene Zellen unterschiedlich berechnet werden. In diesem Fall muss der Benutzer diese Methode überschreiben, damit sie für die Funktion true zurückgibt. Und für [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-), kann der gegebene [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) bereits mit dem zwischengespeicherten Wert der vorherigen Berechnung initialisiert sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionName | java.lang.String | Name der Funktion. In der Regel ist dies der Name der benutzerdefinierten Funktion. Wenn [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) true ist, werden auch integrierte Funktionen hier geprüft. |

**Returns:**
boolescher Wert – true, wenn die angegebene Funktion immer neu berechnet werden muss.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}
```
public boolean getProcessBuiltInFunctions()
```


Gibt an, ob integrierte Funktionen, die von der integrierten Engine unterstützt werden, von dieser Implementierung geprüft und verarbeitet werden sollen. Standardwert ist false.

**Remarks**

Wenn der Benutzer die Berechnungslogik einiger integrierter Funktionen ändern muss, sollte diese Eigenschaft auf true gesetzt werden. Andernfalls lassen Sie diese Eigenschaft bitte aus Leistungsgründen auf false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isParamArrayModeRequired() {#isParamArrayModeRequired--}
```
public boolean isParamArrayModeRequired()
```


Gibt an, ob diese Engine den Parameter im Array‑Modus berechnen muss. Der Standardwert ist false. Wenn [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) beim Berechnen benutzerdefinierter Funktionen erforderlich ist und der Benutzer die Definition dafür nicht aktualisiert hat (mit [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-)), muss diese Eigenschaft auf true gesetzt werden.

**Remarks**

Wenn diese benutzerdefinierte Berechnungs‑Engine den Parameter im Array‑Modus berechnen muss, werden mehr Stacks benötigt, um den Baum für Parameter zu puffern, und die Methode Calculate() kann rekursiv aufgerufen werden, um den Parameterwert zu berechnen. Aus Leistungsgründen behalten Sie diese Eigenschaft bitte beim Standardwert (false) bei, wenn keine besonderen Anforderungen bestehen.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Gibt an, ob diese Engine den Literaltext des Parameters während einer Berechnung benötigt. Der Standardwert ist false.

**Remarks**

Wenn diese benutzerdefinierte Berechnungs‑Engine den Literaltext des Parameters benötigt, werden mehr Stacks benötigt, um den Literaltext für Parameter zu puffern, und die Methode Calculate() kann rekursiv aufgerufen werden, um den Parameterwert zu berechnen. Im Allgemeinen wird der Literaltext für die Berechnung von Formeln nicht benötigt, und diese Eigenschaft sollte für die meisten Implementierungen aus Leistungsgründen auf false belassen werden.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### skipCalculation() {#skipCalculation--}
```
public void skipCalculation()
```


Überspringt die Berechnung der gesamten Formel, die die derzeit ausgewertete Funktion referenziert.

**Remarks**

Diese Methode kann in der Implementierung von [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) aufgerufen werden, um die Berechnung der gesamten Formel zu überspringen, wobei der ursprüngliche Wert der Formel unverändert bleibt.

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

