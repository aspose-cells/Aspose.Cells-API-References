---
title: "AbstractCalculationEngine"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells."
type: docs
url: /sv/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells.

**Remarks**

Användaren bör inte ändra någon del av arbetsboken direkt i denna implementation(förutom det beräknade resultatet av den anpassade funktionen, som kan sättas via egenskapen CalculationData.CalculatedValue). Annars kan oväntade resultat eller undantag uppstå. Om användaren behöver ändra annan data än det beräknade resultatet i implementationen för vissa anpassade funktioner, till exempel ändra cellens formel, stil, ...etc., bör användaren samla dessa data i implementationen och ändra dem utanför formelberäkningens område.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Beräknar en funktion med angivna data. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Om den angivna funktionen ska tvingas att alltid beräknas om vid beräkning av delade formler. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Om inbyggda funktioner som har stöd av den inbyggda motorn ska kontrolleras och bearbetas av denna implementation. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Indikerar om denna motor behöver parametern beräknas i arrayläge. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Indikerar om denna motor behöver den bokstavliga texten för parametern under en beräkning. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Hoppar över beräkningen för hela formeln som refererar till funktionen som för närvarande utvärderas. |
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


Beräknar en funktion med angivna data.

**Remarks**

Användaren bör sätta det beräknade värdet för angivna data för alla funktioner(inklusive Excel‑inbyggda funktioner) som han vill beräkna själv i denna implementation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | de nödvändiga data för att beräkna funktionen såsom funktionsnamn, parametrar, ...etc. |

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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Om den angivna funktionen ska tvingas att alltid beräknas om vid beräkning av delade formler.

**Remarks**

För delade formler delar flera celler samma funktion. Om funktionens parametrar förblir desamma för dessa celler också, behöver funktionen i allmänhet bara beräknas en gång. Så av prestandaskäl beräknar vi sådan typ av funktion bara en gång också([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) anropas bara en gång, istället för att anropas upprepade gånger för varje cell). Däremot, för användarens anpassade implementation kan funktionen, särskilt den anpassade funktionen, behöva beräknas olika för olika celler. I så fall måste användaren åsidosätta denna metod för att få den att returnera true för funktionen. Och för [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-), kan det givna [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) ha initierats med det cachade värdet från föregående beräkning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionName | java.lang.String | namn på funktionen. Vanligtvis är det den anpassade funktionens namn. Om [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) är true, kommer inbyggda funktioner också att kontrolleras här. |

**Returns:**
boolesk - true om den angivna funktionen alltid måste beräknas om.
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


Om inbyggda funktioner som har stöd av den inbyggda motorn ska kontrolleras och bearbetas av denna implementation. Standardvärdet är false.

**Remarks**

Om användaren behöver ändra beräkningslogiken för vissa inbyggda funktioner, bör denna egenskap sättas till true. Annars, vänligen lämna egenskapen som false av prestandaskäl.

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


Anger om den här motorn behöver parametern beräknas i array‑läge. Standardvärdet är falskt. Om [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\\#getParamValueInArrayMode-int-int-int-) krävs vid beräkning av anpassade funktioner och användaren inte har uppdaterat definitionen för dem (via [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\\#updateCustomFunctionDefinition-CustomFunctionDefinition-)), måste den här egenskapen sättas till true.

**Remarks**

Om denna anpassade beräkningsmotor behöver parametern beräknas i array‑läge, kommer fler stackar att behövas för att cachea trädet för parametrar och metoden Calculate() kan anropas rekursivt för att beräkna parameterns värde. Av prestandaskäl, behåll gärna denna egenskap som standardvärdet (false) om det inte finns något särskilt krav.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Anger om den här motorn behöver den bokstavliga texten för parametern under en beräkning. Standardvärdet är falskt.

**Remarks**

Om denna anpassade beräkningsmotor behöver parameterns bokstavliga text, kommer fler stackar att behövas för att cachea den bokstavliga texten för parametrar och metoden Calculate() kan anropas rekursivt för att beräkna parameterns värde. Vanligtvis behövs inte den bokstavliga texten för att beräkna formler och denna egenskap bör hållas på falskt för de flesta implementationer för att få bättre prestanda.

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


Hoppar över beräkningen för hela formeln som refererar till funktionen som för närvarande utvärderas.

**Remarks**

Denna metod kan anropas i implementeringen av [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\\#calculate-CalculationData-) för att hoppa över beräkningen av hela formeln och formelns ursprungliga värde kommer att behållas utan förändring.

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

