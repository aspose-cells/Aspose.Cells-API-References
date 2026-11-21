---
title: "AbstractCalculationMonitor"
second_title: "Aspose.Cells för Java API-referens"
description: "Övervaka så att användaren kan följa framstegen i formelberäkningen."
type: docs
url: /sv/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

Övervaka så att användaren kan följa framstegen i formelberäkningen.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | Implementera den här metoden för att utföra logik efter att en cell har beräknats. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | Implementera den här metoden för att utföra logik innan en cell beräknas. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Hämtar det nyberäknade värdet för cellen. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | Hämtar det gamla värdet för den beräknade cellen. |
| [getValueChanged()](#getValueChanged--) | Om cellens värde har ändrats efter beräkningen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | Implementera den här metoden för att utföra logik när formler med cirkulära referenser beräknas. |
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


Implementera den här metoden för att utföra logik efter att en cell har beräknats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Index för bladet som cellen tillhör. |
| rowIndex | int | Radindex för cellen |
| colIndex | int | Kolumnindex för cellen |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


Implementera den här metoden för att utföra logik innan en cell beräknas.

**Remarks**

För celler i matrisformler kan den här metoden kanske inte köras eftersom dessa celler vanligtvis beräknas tillsammans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Index för bladet som cellen tillhör. |
| rowIndex | int | Radindex för cellen |
| colIndex | int | Kolumnindex för cellen |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


Hämtar det nyberäknade värdet för cellen. Bör endast användas i [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

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


Hämtar det gamla värdet för den beräknade cellen. Bör endast användas i [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) och [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


Om cellens värde har ändrats efter beräkningen. Bör endast användas i [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

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


Implementera den här metoden för att utföra logik när formler med cirkulära referenser beräknas.

**Remarks**

I implementationen kan användaren också ange det förväntade värdet som beräknat resultat för en del/alla av dessa celler så att formelmotorn inte beräknar dem rekursivt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator med [CalculationCell](../../com.aspose.cells/calculationcell)-objekt som representerar celler som beror på cirkulära referenser. |

**Returns:**
boolean - Om formelmotorn behöver beräkna dessa celler i cirkulär ordning efter detta anrop. True för att låta formelmotorn fortsätta beräkna dem. False för att låta formelmotorn bara markera dessa celler som Beräknade.
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

