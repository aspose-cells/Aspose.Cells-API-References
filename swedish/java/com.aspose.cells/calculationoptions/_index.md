---
title: "CalculationOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativ för beräkning."
type: docs
url: /sv/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Representerar alternativ för beräkning.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | Stackstorleken för rekursiv beräkning av celler. |
| [getCalculationMonitor()](#getCalculationMonitor--) | Övervakaren för användaren att följa framstegen i formelberäkning. |
| [getCharacterEncoding()](#getCharacterEncoding--) | Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [getIgnoreError()](#getIgnoreError--) | Anger om fel som uppstår vid beräkning av formler ska ignoreras. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Anger datakällorna för externa länkar som används i formler. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Anger strategin för bearbetning av beräkningsprecision. |
| [getRecursive()](#getRecursive--) | Anger om beroende celler ska beräknas rekursivt när en cell beräknas och den beror på andra celler. |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | Anger om dynamiska arrayformler ska uppdateras innan formler beräknas. |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | Anger om användaren har uttryckligen specificerat beteendet för att uppdatera dynamiska arrayformler innan angivna formler beräknas. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | Stackstorleken för rekursiv beräkning av celler. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | Övervakaren för användaren att följa framstegen i formelberäkning. |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Anger om fel som uppstår vid beräkning av formler ska ignoreras. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Anger datakällorna för externa länkar som används i formler. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Anger strategin för bearbetning av beräkningsprecision. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Anger om beroende celler ska beräknas rekursivt när en cell beräknas och den beror på andra celler. |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | Anger om dynamiska arrayformler ska uppdateras innan formler beräknas. |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


Stackstorleken för rekursiv beräkning av celler. Standardvärdet är 200.

**Remarks**

När ett stort antal celler måste beräknas rekursivt i beroendeträdet kan en StackOverflowException uppstå under beräkningsprocessen. I så fall bör användaren ange ett mindre värde för denna egenskap. I en sådan situation bör användaren bestämma rätt värde för egenskapen baserat på de faktiska formlerna och data. Dock kan ett för litet värde leda till prestandaförsämring för formelberäkningen och ett värde mindre än 2 gör det omöjligt att beräkna en formel som beror på en annan. Så om det angivna värdet är mindre än 2 kommer det att återställas till 2.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


Övervakaren för användaren att följa framstegen i formelberäkning.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. För funktioner som CHAR, CODE beror det beräknade resultatet på regioninställningarna och standardteckenuppsättningen i miljön. Med denna egenskap kan användaren ange rätt kodning som används för dessa funktioner för att få det förväntade resultatet.

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


Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Anger om fel som uppstår vid beräkning av formler ska ignoreras. Felet kan vara en funktion som inte stöds, externa länkar osv. Standardvärdet är true.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Anger datakällorna för externa länkar som används i formler.

**Remarks**

Som [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), kan du här ange datakällor för externa länkar som används i formler som ska beräknas, särskilt de som används i INDIRECT-funktionen. För de externa länkar som används i INDIRECT-funktionen tas de inte med som en del av arbetsbokens externa länkar och kan inte uppdateras av [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). Matchningen av dessa arbetsböcker med externa länkar bestäms av [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) och [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Så se till att [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) har angetts med rätt värde (vanligtvis bör det vara samma som motsvarande [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) för varje arbetsbok så att de kan länkas som förväntat.

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Anger strategin för bearbetning av beräkningsprecision.

Se [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Anger om de beroende cellerna ska beräknas rekursivt när en cell beräknas och den beror på andra celler. Standardvärdet är true.

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


Anger om dynamiska arrayformler ska uppdateras innan formler beräknas.

**Remarks**

Om den här egenskapen har angetts explicit, kommer det angivna värdet att användas för att avgöra om dynamiska arrayformler ska uppdateras. Annars ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) är falskt), beror standardvärdet på vilken typ av formler som behöver beräknas: För beräkning av formler för arbetsboken, såsom [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), kommer denna egenskap att sättas till true. För andra fall, såsom [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) eller [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), kommer egenskapen att sättas till false.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


Anger om användaren har uttryckligen specificerat beteendet för att uppdatera dynamiska arrayformler innan angivna formler beräknas.

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


Stackstorleken för rekursiv beräkning av celler. Standardvärdet är 200.

**Remarks**

När ett stort antal celler måste beräknas rekursivt i beroendeträdet kan en StackOverflowException uppstå under beräkningsprocessen. I så fall bör användaren ange ett mindre värde för denna egenskap. I en sådan situation bör användaren bestämma rätt värde för egenskapen baserat på de faktiska formlerna och data. Dock kan ett för litet värde leda till prestandaförsämring för formelberäkningen och ett värde mindre än 2 gör det omöjligt att beräkna en formel som beror på en annan. Så om det angivna värdet är mindre än 2 kommer det att återställas till 2.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


Övervakaren för användaren att följa framstegen i formelberäkning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


Anger den kodning som används för kodning/avkodning av tecken vid beräkning av formler. För funktioner som CHAR, CODE beror det beräknade resultatet på regioninställningarna och standardteckenuppsättningen i miljön. Med denna egenskap kan användaren ange rätt kodning som används för dessa funktioner för att få det förväntade resultatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Anger om fel som uppstår vid beräkning av formler ska ignoreras. Felet kan vara en funktion som inte stöds, externa länkar osv. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Anger datakällorna för externa länkar som används i formler.

**Remarks**

Som [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), kan du här ange datakällor för externa länkar som används i formler som ska beräknas, särskilt de som används i INDIRECT-funktionen. För de externa länkar som används i INDIRECT-funktionen tas de inte med som en del av arbetsbokens externa länkar och kan inte uppdateras av [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---). Matchningen av dessa arbetsböcker med externa länkar bestäms av [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) och [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--). Så se till att [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) har angetts med rätt värde (vanligtvis bör det vara samma som motsvarande [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--)) för varje arbetsbok så att de kan länkas som förväntat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Anger strategin för bearbetning av beräkningsprecision.

Se [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Anger om de beroende cellerna ska beräknas rekursivt när en cell beräknas och den beror på andra celler. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


Anger om dynamiska arrayformler ska uppdateras innan formler beräknas.

**Remarks**

Om den här egenskapen har angetts explicit, kommer det angivna värdet att användas för att avgöra om dynamiska arrayformler ska uppdateras. Annars ([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) är falskt), beror standardvärdet på vilken typ av formler som behöver beräknas: För beräkning av formler för arbetsboken, såsom [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), kommer denna egenskap att sättas till true. För andra fall, såsom [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) eller [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), kommer egenskapen att sättas till false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

