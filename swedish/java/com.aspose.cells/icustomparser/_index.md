---
title: "ICustomParser"
second_title: "Aspose.Cells för Java API-referens"
description: "Tillåter användare att lägga till sin anpassade värdeparser för att tolka strängvärden till andra lämpliga cellvärdesobjekt."
type: docs
url: /sv/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

Tillåter användare att lägga till sin anpassade värdeparser för att tolka strängvärden till andra lämpliga cellvärdesobjekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFormat()](#getFormat--) | Hämtar formateringsmönstret som motsvarar det analyserade värdet från den senaste anropet av [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-). |
| [parseObject(String value)](#parseObject-java.lang.String-) | Analyserar den givna strängen till ett korrekt värdeobjekt. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Hämtar formateringsmönstret som motsvarar det analyserade värdet från den senaste anropet av [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-).

**Remarks**

Det returnerade formateringsmönstret kan användas för att formatera motsvarande cell (sätt till Style.Custom för cellen).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


Analyserar den givna strängen till ett korrekt värdeobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | Strängvärdet som ska parsas |

**Returns:**
java.lang.Object - Parsat värdeobjekt från given sträng. Om given sträng inte kan parsas till ett korrekt värdeobjekt, returneras null.
