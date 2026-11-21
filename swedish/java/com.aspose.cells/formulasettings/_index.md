---
title: "FormulaSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Inställningar för formler och beräkning."
type: docs
url: /sv/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Inställningar för formler och beräkning.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Anger om arbetsboken ska beräknas om innan dokumentet sparas, när man är i manuellt beräkningsläge. |
| [getCalculationId()](#getCalculationId--) | Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken. |
| [getCalculationMode()](#getCalculationMode--) | Hämtar läget för arbetsboksberäkning i MS Excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Anger om beräkningskedjan för formler ska aktiveras. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Anger om alla formler beräknas varje gång en beräkning utlöses. |
| [getMaxChange()](#getMaxChange--) | Den maximala förändringen för att lösa en cirkulär referens. |
| [getMaxIteration()](#getMaxIteration--) | Det maximala antalet iterationer för att lösa en cirkulär referens. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Anger om precisionen för beräknat resultat ska sättas enligt hur de visas under beräkning av formler. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | Anger om mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas. |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | Anger om arbetsboken ska beräknas om innan dokumentet sparas, när man är i manuellt beräkningsläge. |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Ställer in läget för arbetsboksberäkning i MS Excel. |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | Anger om beräkningskedjan för formler ska aktiveras. |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser. |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | Anger om alla formler beräknas varje gång en beräkning utlöses. |
| [setMaxChange(double value)](#setMaxChange-double-) | Den maximala förändringen för att lösa en cirkulär referens. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Det maximala antalet iterationer för att lösa en cirkulär referens. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | Anger om precisionen för beräknat resultat ska sättas enligt hur de visas under beräkning av formler. |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | Anger om mellanslag och radbrytningar som är insatta mellan formeltoken ska bevaras vid hämtning och inställning av formler. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Anger om arbetsboken ska beräknas om innan dokumentet sparas, när man är i manuellt beräkningsläge.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas och manipuleras. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas och manipuleras. I fallet med MS Excel, om värdet för denna egenskap är mindre än identifieraren för återberäkningsmotorn som är associerad med programmet som öppnar den resulterande filen, kommer programmet att beräkna om resultaten för alla formler i arbetsboken omedelbart efter att filen har laddats. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


Hämtar läget för arbetsboksberäkning i MS Excel.

Se [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom ms excel) kan agera därefter när de laddar och manipulerar den resulterande filen. Av prestandaskäl för de flesta användares applikation beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket läge som har ställts in för denna egenskap. Om användaren behöver beräkna formler, vänligen anropa alltid metoder på olika objekt enligt krav: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

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


Anger om beräkningskedjan för formler ska aktiveras. Standard är falskt.

**Remarks**

När det finns många formler i arbetsboken och användaren behöver beräkna dem upprepade gånger genom att bara ändra en liten del av dem, kan det vara hjälpsamt för prestandan att aktivera beräkningskedjan. Å andra sidan, om kedjan är aktiverad kräver underhållet av kedjemodellen extra minne, och det kräver också lite mer CPU-tid för vissa andra operationer såsom att ändra cellens värde eller formler. Efter att ha ändrat denna egenskap från falskt till sant kommer beräkningskedjan att analyseras och byggas vid den första beräkningen av arbetsboken, så den tid som krävs för den första beräkningen kan bli längre än en normal beräkning utan kedja.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Anger om alla formler beräknas varje gång en beräkning utlöses.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas och manipuleras. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


Den maximala förändringen för att lösa en cirkulär referens.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Det maximala antalet iterationer för att lösa en cirkulär referens.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Anger om precisionen för beräknat resultat ska sättas enligt hur de visas under beräkning av formler.

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


Anger om de mellanslag och radbrytningar som är insatta mellan formeltoken vid hämtning och inställning av formler ska bevaras. Standardvärdet är falskt.

**Remarks**

Generellt är dessa mellanslag och radbrytningar bara för visuell presentation, att bevara dem eller inte påverkar inte det beräknade resultatet. Av prestandaskäl, om det inte finns något särskilt krav, är det bättre att inte bevara dem vid bearbetning av formler.

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


Anger om applikationen måste utföra en fullständig beräkning när arbetsboken öppnas.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


Anger om arbetsboken ska beräknas om innan dokumentet sparas, när man är i manuellt beräkningsläge.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas och manipuleras. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


Anger versionen av beräkningsmotorn som används för att beräkna värden i arbetsboken.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas och manipuleras. I fallet med MS Excel, om värdet för denna egenskap är mindre än identifieraren för återberäkningsmotorn som är associerad med programmet som öppnar den resulterande filen, kommer programmet att beräkna om resultaten för alla formler i arbetsboken omedelbart efter att filen har laddats. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


Ställer in läget för arbetsboksberäkning i MS Excel.

Se [CalcModeType](../../com.aspose.cells/calcmodetype).

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom ms excel) kan agera därefter när de laddar och manipulerar den resulterande filen. Av prestandaskäl för de flesta användares applikation beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket läge som har ställts in för denna egenskap. Om användaren behöver beräkna formler, vänligen anropa alltid metoder på olika objekt enligt krav: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


Anger om beräkningskedjan för formler ska aktiveras. Standard är falskt.

**Remarks**

När det finns många formler i arbetsboken och användaren behöver beräkna dem upprepade gånger genom att bara ändra en liten del av dem, kan det vara hjälpsamt för prestandan att aktivera beräkningskedjan. Å andra sidan, om kedjan är aktiverad kräver underhållet av kedjemodellen extra minne, och det kräver också lite mer CPU-tid för vissa andra operationer såsom att ändra cellens värde eller formler. Efter att ha ändrat denna egenskap från falskt till sant kommer beräkningskedjan att analyseras och byggas vid den första beräkningen av arbetsboken, så den tid som krävs för den första beräkningen kan bli längre än en normal beräkning utan kedja.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


Anger om iterativ beräkning ska aktiveras för att lösa cirkulära referenser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


Anger om alla formler beräknas varje gång en beräkning utlöses.

**Remarks**

Denna egenskap är endast för att spara inställningarna till den resulterande kalkylbladsfilen så att andra program (såsom MS Excel) kan agera därefter när den resulterande filen laddas och manipuleras. Med hänsyn till prestanda för de flesta användares applikationer beräknar vi inte någon formel i arbetsboken automatiskt, oavsett vilket värde som har satts för denna egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


Den maximala förändringen för att lösa en cirkulär referens.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Det maximala antalet iterationer för att lösa en cirkulär referens.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


Anger om precisionen för beräknat resultat ska sättas enligt hur de visas under beräkning av formler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


Anger om de mellanslag och radbrytningar som är insatta mellan formeltoken vid hämtning och inställning av formler ska bevaras. Standardvärdet är falskt.

**Remarks**

Generellt är dessa mellanslag och radbrytningar bara för visuell presentation, att bevara dem eller inte påverkar inte det beräknade resultatet. Av prestandaskäl, om det inte finns något särskilt krav, är det bättre att inte bevara dem vid bearbetning av formler.

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

