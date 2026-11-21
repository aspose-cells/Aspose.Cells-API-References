---
title: "FindOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar sökalternativ."
type: docs
url: /sv/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Representerar sökalternativ.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Anger om den sökta strängen är skiftlägeskänslig. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Hämtar ett värde som anger om den sökta strängvärdet ska konverteras till numerisk data. |
| [getLookAtType()](#getLookAtType--) | Titta på typ. |
| [getLookInType()](#getLookInType--) | Sök i typ. |
| [getRange()](#getRange--) | Hämtar och anger det sökta intervallet. |
| [getRegexKey()](#getRegexKey--) | Anger om den sökta nyckeln är ett regex. |
| [getSearchBackward()](#getSearchBackward--) | Om sökningen ska gå bakåt för celler. |
| [getSearchNext()](#getSearchNext--) | Sökordning. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Anger om sökordningen är efter rader eller kolumner. |
| [getStyle()](#getStyle--) | Formatet att söka efter. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Anger om den sökta cellvärdestypen ska vara samma som den sökta nyckeln. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Anger om det sökta intervallet är angivet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Anger om den sökta strängen är skiftlägeskänslig. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Anger ett värde som visar om den sökta strängvärdet ska konverteras till numerisk data. |
| [setLookAtType(int value)](#setLookAtType-int-) | Titta på typ. |
| [setLookInType(int value)](#setLookInType-int-) | Sök i typ. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Anger det sökta intervallet. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Anger om den sökta nyckeln är ett regex. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Om sökningen ska gå bakåt för celler. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Sökordning. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Anger om sökordningen är efter rader eller kolumner. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Formatet att söka efter. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Anger om den sökta cellvärdestypen ska vara samma som den sökta nyckeln. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Anger om den sökta strängen är skiftlägeskänslig.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Hämtar ett värde som anger om den sökta strängvärdet ska konverteras till numerisk data.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Titta på typ.

Se [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

När [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) är true och användaren har specificerat den exakta regeln för regex, bör denna egenskap av prestandaskäl sättas till [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Annars kommer vi att omstrukturera söknyckeln för att säkerställa att den kan matchas enligt den specifika typen. Till exempel, när typen är [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (detta är standardvärdet för denna egenskap), kommer vi automatiskt att lägga till jokertecken i början och slutet av söknyckeln. I detta fall blir de reguljära uttrycken mer komplexa och prestandan minskar också.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


Sök i typ.

Se [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


Hämtar och anger det sökta intervallet.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


Anger om den sökta nyckeln är ett regex. Om true tas den sökta nyckeln som regex och tolkas. Annars kommer nyckeln att tolkas enligt reglerna i MS Excel.

**Remarks**

Även om söknyckeln har specificerats som regex kan den omstruktureras enligt den angivna [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). Till exempel, när typen är [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (detta är standardvärdet för dessa alternativ), kommer jokertecken att läggas till i början och slutet av söknyckeln automatiskt för att säkerställa att matchningen kontrolleras som \"contains\". I detta fall blir de reguljära uttrycken mer komplexa och prestandan minskar också. Så, av prestandaskäl, om användaren har specificerat den exakta regeln för regex, finns det inget behov av att använda [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) som ytterligare begränsning och användaren kan sätta den till [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) för att få bättre prestanda.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


Om sökningen ska gå bakåt för celler.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


Sökordning. True: sök nästa. False: sök föregående.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället FindOptions.SearchBackward property. Denna egenskap kommer att tas bort 12 månader senare sedan november 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


Anger om sökordningen är efter rader eller kolumner.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Formatet att söka efter.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


Anger om den sökta cellvärdestypen ska vara samma som den sökta nyckeln.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


Anger om det sökta intervallet är angivet.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Anger om den sökta strängen är skiftlägeskänslig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Anger ett värde som visar om den sökta strängvärdet ska konverteras till numerisk data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


Titta på typ.

Se [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

När [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) är true och användaren har specificerat den exakta regeln för regex, bör denna egenskap av prestandaskäl sättas till [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Annars kommer vi att omstrukturera söknyckeln för att säkerställa att den kan matchas enligt den specifika typen. Till exempel, när typen är [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (detta är standardvärdet för denna egenskap), kommer vi automatiskt att lägga till jokertecken i början och slutet av söknyckeln. I detta fall blir de reguljära uttrycken mer komplexa och prestandan minskar också.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


Sök i typ.

Se [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


Anger det sökta intervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | det sökta intervallet. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


Anger om den sökta nyckeln är ett regex. Om true tas den sökta nyckeln som regex och tolkas. Annars kommer nyckeln att tolkas enligt reglerna i MS Excel.

**Remarks**

Även om söknyckeln har specificerats som regex kan den omstruktureras enligt den angivna [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). Till exempel, när typen är [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (detta är standardvärdet för dessa alternativ), kommer jokertecken att läggas till i början och slutet av söknyckeln automatiskt för att säkerställa att matchningen kontrolleras som \"contains\". I detta fall blir de reguljära uttrycken mer komplexa och prestandan minskar också. Så, av prestandaskäl, om användaren har specificerat den exakta regeln för regex, finns det inget behov av att använda [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) som ytterligare begränsning och användaren kan sätta den till [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) för att få bättre prestanda.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


Om sökningen ska gå bakåt för celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


Sökordning. True: sök nästa. False: sök föregående.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället FindOptions.SearchBackward property. Denna egenskap kommer att tas bort 12 månader senare sedan november 2018. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


Anger om sökordningen är efter rader eller kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Formatet att söka efter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


Anger om den sökta cellvärdestypen ska vara samma som den sökta nyckeln.

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

