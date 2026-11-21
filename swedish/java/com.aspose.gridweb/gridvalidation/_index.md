---
title: "GridValidation"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar data validation.settings."
type: docs
url: /sv/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

Representerar data validation.settings.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ServerValidation](#ServerValidation) | Hämtar eller anger serversidans validerings‑javascript‑funktionsnamn. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | lägg till valideringsinställningarna i cellen. |
| [addACell(String cellname)](#addACell-java.lang.String-) | lägg till valideringsinställningarna i cellen. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Tillämpar valideringen på området. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Representerar en samling av [GridCellArea](../../com.aspose.gridweb/gridcellarea) som innehåller datavalideringsinställningarna. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | Hämtar klientens validerings‑javascript‑funktionsnamn. |
| [getErrorMessage()](#getErrorMessage--) | Representerar felmeddelandet för datavalidering. |
| [getErrorTitle()](#getErrorTitle--) | Representerar titeln på felmeddelanderutan för datavalidering. |
| [getFormula1()](#getFormula1--) | Representerar värdet eller uttrycket som är kopplat till datavalideringen. |
| [getFormula2()](#getFormula2--) | Representerar värdet eller uttrycket som är associerat med den andra delen av datavalideringen. |
| [getInputMessage()](#getInputMessage--) | Representerar felmeddelandet för datavalidering. |
| [getInputTitle()](#getInputTitle--) | Representerar titeln på datavalideringens inmatningsdialogruta. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Hämta värdet för listan av valideringen för den angivna cellen. |
| [getOperator()](#getOperator--) | Representerar operatorn för datavalideringen. |
| [getRegEx()](#getRegEx--) | Hämtar reguljära uttryckets sträng. |
| [getShowError()](#getShowError--) | Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data. |
| [getShowInput()](#getShowInput--) | Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet. |
| [getValidationType()](#getValidationType--) | Hämtar valideringstypen. |
| [getValue1()](#getValue1--) | Representerar värdet som är associerat med datavalideringen. |
| [getValueList()](#getValueList--) | Hämtar värdelistobjektet. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Hämtar om cellvärdet är obligatoriskt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Ta bort valideringsinställningarna i cellen. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Ta bort valideringsinställningarna i området. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | Anger klientens validerings‑javascript‑funktionsnamn. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Representerar felmeddelandet för datavalidering. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Representerar titeln på felmeddelanderutan för datavalidering. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Representerar värdet eller uttrycket som är kopplat till datavalideringen. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Representerar värdet eller uttrycket som är associerat med den andra delen av datavalideringen. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Representerar felmeddelandet för datavalidering. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Representerar titeln på datavalideringens inmatningsdialogruta. |
| [setOperator(int value)](#setOperator-int-) | Representerar operatorn för datavalideringen. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Anger reguljära uttryckets sträng. |
| [setRequired(boolean value)](#setRequired-boolean-) | Anger om cellvärdet är obligatoriskt. |
| [setShowError(boolean value)](#setShowError-boolean-) | Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet. |
| [setValidationType(int value)](#setValidationType-int-) | Anger valideringstypen. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Anger värdelistobjektet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Hämtar eller anger serversidans validerings‑javascript‑funktionsnamn.

**Remarks**

Använd egenskapen GridCustomServerValidation för att ange serversidig validering.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


lägg till valideringsinställningarna i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


lägg till valideringsinställningarna i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellname | java.lang.String | cellnamn. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


Tillämpar valideringen på området.

**Remarks**

I den här metoden kommer vi att ta bort alla gamla valideringar i detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Området. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


Representerar en samling av [GridCellArea](../../com.aspose.gridweb/gridcellarea) som innehåller datavalideringsinställningarna.

**Remarks**

De gamla valideringarna i området kommer inte att tas bort om du lägger till direkt i den här listan.

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


Hämtar klientens validerings‑javascript‑funktionsnamn.

**Remarks**

Använd egenskapen ClientValidationFunction för att ange namn på klientvalideringsfunktionen. Funktionen bör deklareras enligt detta format:
function customValicationFunction(source, value)
Parametern "source" är cellobjektet. Parametern "value" är cellens strängvärde som ska kontrolleras. Funktionen bör returnera sant om värdet är giltigt.

**Returns:**
java.lang.String
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


Representerar felmeddelandet för datavalidering.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Representerar titeln på felmeddelanderutan för datavalidering.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Representerar värdet eller uttrycket som är kopplat till datavalideringen.

**Returns:**
java.lang.String
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Representerar värdet eller uttrycket som är associerat med den andra delen av datavalideringen.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Representerar felmeddelandet för datavalidering.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Representerar titeln på datavalideringens inmatningsdialogruta.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Hämta värdet för listan av valideringen för den angivna cellen.

**Remarks**

Endast för validering vars typ är List och som har tillämpats på den angivna cellen, annars returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.Object - Värdet för att producera listan av denna validering för den angivna cellen. Om listan refererar till ett område kommer det returnerade värdet att vara ett ReferredArea-objekt; annars kan det returnerade värdet vara null, object[] eller ett enkelt objekt.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Representerar operatorn för datavalideringen.

Se [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


Hämtar reguljära uttryckets sträng.

**Returns:**
java.lang.String
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet.

**Returns:**
boolean
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


Hämtar valideringstypen.

Se [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


Representerar värdet som är associerat med datavalideringen.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


Hämtar värdelistobjektet.

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


Hämtar om cellvärdet är obligatoriskt.

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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Ta bort valideringsinställningarna i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


Ta bort valideringsinställningarna i området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Området som innehåller inställningarna för datavalidering. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


Anger klientens validerings‑javascript‑funktionsnamn.

**Remarks**

Använd egenskapen ClientValidationFunction för att ange namn på klientvalideringsfunktionen. Funktionen bör deklareras enligt detta format:
function customValicationFunction(source, value)
Parametern "source" är cellobjektet. Parametern "value" är cellens strängvärde som ska kontrolleras. Funktionen bör returnera sant om värdet är giltigt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Representerar felmeddelandet för datavalidering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Representerar titeln på felmeddelanderutan för datavalidering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Representerar värdet eller uttrycket som är kopplat till datavalideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Representerar värdet eller uttrycket som är associerat med den andra delen av datavalideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Representerar felmeddelandet för datavalidering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Representerar titeln på datavalideringens inmatningsdialogruta.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Representerar operatorn för datavalideringen.

Se [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


Anger reguljära uttryckets sträng.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


Anger om cellvärdet är obligatoriskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


Anger valideringstypen.

Se [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


Anger värdelistobjektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.ArrayList<java.lang.String> |  |

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

