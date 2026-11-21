---
title: "FormulaParseOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativ vid tolkning av formel."
type: docs
url: /sv/java/com.aspose.cells/formulaparseoptions/
---

**Inheritance:**
java.lang.Object
```
public class FormulaParseOptions
```

Representerar alternativ vid tolkning av formel.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [FormulaParseOptions()](#FormulaParseOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckAddIn()](#getCheckAddIn--) | Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. |
| [getClass()](#getClass--) |  |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--) | Definition för att tolka anpassade funktioner. |
| [getLocaleDependent()](#getLocaleDependent--) | Om formeln är lokalanpassad. |
| [getParse()](#getParse--) | Om given formel ska tolkas. |
| [getR1C1Style()](#getR1C1Style--) | Om formeln är i R1C1-referensstil. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckAddIn(boolean value)](#setCheckAddIn-boolean-) | Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. |
| [setCustomFunctionDefinition(CustomFunctionDefinition value)](#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Definition för att tolka anpassade funktioner. |
| [setLocaleDependent(boolean value)](#setLocaleDependent-boolean-) | Om formeln är lokalanpassad. |
| [setParse(boolean value)](#setParse-boolean-) | Om given formel ska tolkas. |
| [setR1C1Style(boolean value)](#setR1C1Style-boolean-) | Om formeln är i R1C1-referensstil. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FormulaParseOptions() {#FormulaParseOptions--}
```
public FormulaParseOptions()
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
### getCheckAddIn() {#getCheckAddIn--}
```
public boolean getCheckAddIn()
```


Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. Standard är true (om en användardefinierad funktion matchar ett tillägg i befintliga externa länkar, tas den som tillägget).

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```
public CustomFunctionDefinition getCustomFunctionDefinition()
```


Definition för att tolka anpassade funktioner.

**Remarks**

För vissa speciella krav, till exempel när en anpassad funktion beräknas i användarens egna motor, måste vissa parametrar beräknas i arrayläge; med den här egenskapen kan dessa parametrar markeras som arrayläge vid tolkning av formeln. Annars måste användaren uppdatera de anpassade funktionerna senare via [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) för att få samma resultat.

**Returns:**
[CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition)
### getLocaleDependent() {#getLocaleDependent--}
```
public boolean getLocaleDependent()
```


Om formeln är lokalanpassad. Standard är false.

**Returns:**
boolean
### getParse() {#getParse--}
```
public boolean getParse()
```


Om formeln ska tolkas. Standard är true. Om den är false kommer den givna formelsträngen att behållas oförändrad för cellen tills användaren anropar andra metoder för att tolka dem eller tolkad formeldatat krävs av andra operationer såsom beräkning av formler.

**Returns:**
boolean
### getR1C1Style() {#getR1C1Style--}
```
public boolean getR1C1Style()
```


Om formeln är i R1C1-referensstil. Standard är false.

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




### setCheckAddIn(boolean value) {#setCheckAddIn-boolean-}
```
public void setCheckAddIn(boolean value)
```


Om tillägg ska kontrolleras i befintliga externa länkar i den aktuella arbetsboken för användardefinierade funktioner utan extern länk. Standard är true (om en användardefinierad funktion matchar ett tillägg i befintliga externa länkar, tas den som tillägget).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCustomFunctionDefinition(CustomFunctionDefinition value) {#setCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void setCustomFunctionDefinition(CustomFunctionDefinition value)
```


Definition för att tolka anpassade funktioner.

**Remarks**

För vissa speciella krav, till exempel när en anpassad funktion beräknas i användarens egna motor, måste vissa parametrar beräknas i arrayläge; med den här egenskapen kan dessa parametrar markeras som arrayläge vid tolkning av formeln. Annars måste användaren uppdatera de anpassade funktionerna senare via [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) för att få samma resultat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) |  |

### setLocaleDependent(boolean value) {#setLocaleDependent-boolean-}
```
public void setLocaleDependent(boolean value)
```


Om formeln är lokalanpassad. Standard är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setParse(boolean value) {#setParse-boolean-}
```
public void setParse(boolean value)
```


Om formeln ska tolkas. Standard är true. Om den är false kommer den givna formelsträngen att behållas oförändrad för cellen tills användaren anropar andra metoder för att tolka dem eller tolkad formeldatat krävs av andra operationer såsom beräkning av formler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setR1C1Style(boolean value) {#setR1C1Style-boolean-}
```
public void setR1C1Style(boolean value)
```


Om formeln är i R1C1-referensstil. Standard är false.

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

